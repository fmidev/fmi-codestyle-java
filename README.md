# FMI Java Code Style Rules

Following rules for FMI Java code are provided:

* [Checkstyle](https://checkstyle.org/) (for Checkstyle version 7.x.x,
  version >= 8 is not yet supported) 



## Applying rules in IntelliJ IDEA

In addition to instructions below, apply the code style rules distributed in the
[fmi-codestyle-idea](https://github.com/fmidev/fmi-codestyle-idea) repository.

### Checkstyle rules

1. Install [CheckStyle-IDEA plugin](https://github.com/jshiell/checkstyle-idea)
   under **Plugins** in the **Settings/Preferences** dialog.
2. In the **Settings/Preferences** dialog, click **Checkstyle** under
      **Other settings**.
3. Select latest Checkstyle version supported by FMI rules.
   Checkstyle version >=8 is not yet supported.
4. Select **Only Java sources (but not tests)** for Scan Scope.
5. Add a new configuration file by clicking `+` button.
   1. Description: **FMI**
   2. **Use a Checkstyle file accessible via HTTP** \
      URL: <https://raw.githubusercontent.com/fmidev/fmi-codestyle-java/master/src/main/resources/fi/fmi/codestyle/checkstyle/fmi-checkstyle-config.xml>
   3. Click **Next** and set property:
      * Property Name: `checkstyle.suppressions.file`
      * Value: <https://raw.githubusercontent.com/fmidev/fmi-codestyle-java/master/src/main/resources/fi/fmi/codestyle/checkstyle/fmi-checkstyle-suppressions.xml>
   4. Click **Next**, then click **Finish**.
6. Check
   * [X] **FMI**
6. Click OK.

If you're mainly working with FMI code, you should consider configuring the
rules in the **Project Defaults | Settings** dialog.
