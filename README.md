# @wharfkit/account-creation-plugin-template

A template to create a `account-creationPlugin` for use within the `@wharfkit/session` library.

## Usage

-   [Use this as a template.](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)
-   Write your account-creation plugin's logic. For more information on how to do this, see the [Wharf Account Creation Plugin Documentation](https://wharfkit.com/docs/session-kit/plugin-account-creation)
-   Publish it on Github or npmjs.com
-   Include it in your Wharf project and use it:

```ts
    import { SessionKit } from "@wharfkit/session";
    import { YourAccountCreationPlugin } from "your-account-creation-plugin";

    const sessionKit = new SessionKit(
        {
            accountCreationPlugins: [new YourAccountCreationPlugin()],
        }
    );
```

## Developing

You need [Make](https://www.gnu.org/software/make/), [node.js](https://nodejs.org/en/) and [yarn](https://classic.yarnpkg.com/en/docs/install) installed.

Clone the repository and run `make` to checkout all dependencies and build the project. See the [Makefile](./Makefile) for other useful targets. Before submitting a pull request make sure to run `make lint`.

---

Made with ☕️ & ❤️ by [Greymass](https://greymass.com), if you find this useful please consider [supporting us](https://greymass.com/support-us).
