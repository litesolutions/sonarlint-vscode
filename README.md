# SonarLint for Visual Studio Code

SonarLint is an IDE extension that helps you detect and fix quality issues as you write code. Like a spell checker, SonarLint squiggles flaws so they can be fixed before committing code. You can get it directly from the VS Code Marketplace and it will then detect new bugs and quality issues as you code (ObjectScript and JavaScript)

## How it works

Simply open a INT, MAC, CLS or JS file, start coding, and you will start seeing issues reported by SonarLint. Issues are highlighted in your code, and also listed in the 'Problems' panel.

![sonarlint on-the-fly](images/sonarlint-vscode.gif)

You can access the detailed rule description directly from your editor, using the provided contextual menu.

![rule description](images/sonarlint-rule-description.gif)

## Rules

Check the rules to see what SonarLint can do for you:

- [ObjectScript rules](https://www.cachequality.com/docs/cachequality-release/rules)
- [JavaScript rules](https://rules.sonarsource.com/javascript)

You will benefit from the following code analyzers: [CacheQuality](https://www.cachequality.com) and [SonarJS](https://redirect.sonarsource.com/plugins/javascript.html)

## Requirements

The only thing you need is a Java Runtime (JRE) 8 installed on your computer.

SonarLint should automatically find it but you can also explicitly set the path where the JRE is installed using the 'sonarlint.ls.javaHome' variable in VS Code settings. For example:

    {
        "sonarlint.ls.javaHome": "C:\Program Files\Java\jre1.8.0_131"
    }

### Connected mode

You can connect SonarLint to SonarQube >= 5.6 or SonarCloud to benefit from the same rules and settings that are used to inspect your project on the server. SonarLint then hides in VSCode the issues that are marked as **Won’t Fix** or **False Positive**.

To configure the connection, have a look at SonarLint in default user settings.

If you change something on the server such as the quality profile, you can trigger an update of the local cache using the "Update SonarLint binding to SonarQube/SonarCloud" command on the command palette (search for "sonarlint").

For security reasons, the token should not be stored in SCM with workspace settings.

## Contributions and license

SonarLint for Visual Studio Code is open source under the LGPL v3 license. Feel free to submit Pull Requests.

## Feedback

The preferred way to discuss about VS SonarLint for CacheQuality is by posting on the [Project Issues tab](https://github.com/litesolutions/cachequality-vscode/issues). Feel free to ask questions, report issues, and give suggestions.
