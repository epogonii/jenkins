### [Jenkins](https://www.jenkins.io)

The theme is the [Dracula Theme](https://plugins.jenkins.io/dracula-theme/) plugin. It needs Jenkins 2.541.3 or newer. The [Theme Manager](https://plugins.jenkins.io/theme-manager/) plugin is installed with it as a dependency.

#### Install from the Update Center

1. Go to **Manage Jenkins** → **Plugins** → **Available plugins**;
2. Search for `Dracula Theme`, select it and click **Install**.

#### Install manually

1. Download the latest `dracula-theme.hpi` from the [plugin releases page](https://plugins.jenkins.io/dracula-theme/releases/);
2. Go to **Manage Jenkins** → **Plugins** → **Advanced settings**;
3. Under **Deploy Plugin**, choose the `.hpi` file and click **Deploy**.

#### Activating theme

1. Go to **Manage Jenkins** → **Appearance**;
2. Select **Dracula** and click **Save**;
3. Boom! It's working ✨

To use Dracula for every user, also select **Do not allow users to select a different theme**. Otherwise, each user can select **Dracula** in their user menu → **Appearance**.

#### Configuration as Code

With the [Configuration as Code](https://plugins.jenkins.io/configuration-as-code/) plugin:

```yaml
appearance:
  themeManager:
    disableUserThemes: true
    theme: "dracula"
```
