```text
#Directory.Build.props

Here is what each setting does:

Nullable: Enables nullable reference types, which help prevent null reference exceptions. The compiler warns you when you might be using a null value incorrectly.

ImplicitUsings: Adds common namespace imports to every file. You don't need to write using System; or using System.Linq; anymore.

AnalysisLevel: Sets the code analysis level to the latest version. You get the most recent code quality checks from Microsoft.

AnalysisMode: Turns on all code analysis rules. This gives you the most feedback on code quality.

TreatWarningsAsErrors: Stops compilation if there are any warnings. This forces you to fix issues right away instead of letting them pile up.

CodeAnalysisTreatWarningsAsErrors: Applies the same strict treatment to code analysis warnings.

EnforceCodeStyleInBuild: Runs code style checks during build, not just in the IDE. Your CI/CD pipeline will catch style violations.

```

```text
#Directory.Build.props

Here is what each setting does:

Nullable: Enables nullable reference types, which help prevent null reference exceptions. The compiler warns you when you might be using a null value incorrectly.

ImplicitUsings: Adds common namespace imports to every file. You don't need to write using System; or using System.Linq; anymore.

AnalysisLevel: Sets the code analysis level to the latest version. You get the most recent code quality checks from Microsoft.

AnalysisMode: Turns on all code analysis rules. This gives you the most feedback on code quality.

TreatWarningsAsErrors: Stops compilation if there are any warnings. This forces you to fix issues right away instead of letting them pile up.

CodeAnalysisTreatWarningsAsErrors: Applies the same strict treatment to code analysis warnings.

EnforceCodeStyleInBuild: Runs code style checks during build, not just in the IDE. Your CI/CD pipeline will catch style violations.

SonarAnalyzer.CSharp: Focuses on code quality, security holes, and code smells. It finds complex methods, duplicated code, and potential bugs.

Meziantou.Analyzer: Catches performance issues, security holes, and incorrect API usage. It has hundreds of rules covering async/await patterns, LINQ usage, string handling, and more.

Roslynator.Analyzers: Provides code analysis and refactoring suggestions. It helps you write cleaner, more idiomatic C# code.

xunit.analyzers: Makes sure you write tests correctly. It catches common testing mistakes, such as missing assertions or wrong test attributes.

The IncludeAssets configuration makes sure that these analyzers run during compilation but don't get included in your published application.

With TreatWarningsAsErrors enabled, your build will fail if any analyzer finds an issue. This might seem strict, but it stops technical debt from piling up.

You should always aim for zero warnings in your project. Many developers ignore warnings, but warnings often point at real problems that will cause bugs later.

These four packages carry thousands of rules between them. That's thousands of rules an AI agent has to satisfy, and none of them cost you a single line in a prompt.

```


``` text
#.editorconfig

The .editorconfig file defines coding standards and sets the severity level for each analyzer rule. You can mark rules as errors, warnings, suggestions, or turn them off completely.

```


``` text
 Directory.Packages.props

```
