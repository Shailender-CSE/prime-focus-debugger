# prime-focus-debugger
Prime Focus Debugger is a multi‑language tool that detects Python and C errors, explains them clearly, and provides corrected code. With a modular design and Gradio UI, it helps learners focus on problem‑solving instead of deciphering confusing compiler messages.

📌 Overview
Prime Focus is a multi‑language debugging tool built to help developers quickly identify and resolve errors in both Python and C programs. It provides structured error reports, suggested fixes, and corrected code snippets through an easy‑to‑use Gradio web interface.

✨ Features
Language Detection: Automatically distinguishes between Python and C code.

Python Debugging:

Detects syntax errors (e.g., missing parentheses, indentation issues).

Classifies runtime errors (e.g., NameError, TypeError).

Optional linting with flake8 for style issues.

Provides suggested fixes and corrected code.

C Debugging:

Compiles code with GCC and captures warnings/errors.

Parses compiler messages into structured issues.

Suggests fixes for common problems (e.g., missing semicolons, undeclared variables, missing return).

Produces corrected code with basic auto‑patches.

Gradio Interface:

Paste code directly into the textbox.

View Language, Category, Detail, Suggestion, Corrected Code in separate fields.

Shareable public link for demonstrations.

🚀 How It Works
Paste your code into the Gradio textbox.

The tool detects the programming language.

Runs the appropriate debugging process:

Python → Lint + Runtime analysis.

C → GCC compile + static checks.

Displays results:

Error category

Detailed message

Suggested fix

Corrected code

🛠️ Tech Stack
Python 3.x

Gradio (UI framework)

Subprocess + GCC (for C compilation)

AST + Traceback (for Python error parsing)

Optional Flake8 (Python linting)

📂 Project Structure
debug_c_code() → Handles C compilation, parsing, and fixes.

debug_python_code() → Handles Python linting, runtime errors, and fixes.

handle_debug() → Unified handler with language detection.

Gradio UI → User interface for interaction and demo.

🎯 Use Cases
Students learning programming (Python/C).

Developers needing quick error feedback.

Demonstrations of debugging workflows.

Portfolio project showcasing practical error handling.

✅ Future Improvements
Expand language support (Java, JavaScript).

Smarter auto‑patching with AST transformations.

Persistent session logging for error analysis.

Deploy permanent demo on Hugging Face Spaces.

📖 Author
Developed by Shailender — combining academic consistency, sports discipline, and technical problem‑solving into a practical debugging tool.
