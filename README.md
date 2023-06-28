# React-Ios-Android-Native-Xcode-AndroidStudio-Starter-Webapp
React Ios and Android Native web application stater template for quick development and optimized with ionic themes: Run npm install, npm run dev, npm run ionic:buiild and npm run ionic:serve make sure sure to have android studio, xcode and nodejs on your computer.

<h1>Mannaul Installation</h1>

 Vite, React, Ionic, and Capacitor are all great tools for building modern Navtive web apps. Let's get everything installed. Here's a step-by-step guide:

**Step 1: Install Node.js and npm**

Before you can use Vite, React, Ionic, or Capacitor, you'll need to have Node.js and npm installed on your system. You can download Node.js from the [official website](https://nodejs.org/). npm is included as part of Node.js.

**Step 2: Install Vite**

Once you have Node.js and npm installed, you can install Vite by running the following command in your terminal:

```
npm install create-vite
```

**Step 3: Create a new Vite + React project**

Now you can use Vite to create a new project. You'll use the `create-vite` command, specify your project name (replace `my-vite-project` with your actual project name), and then specify that you want to use the React template:

```
npx create-vite my-vite-project --template react
```

**Step 4: Navigate to your new project directory**

Move to the newly created project directory with:

```
cd my-vite-project
```

**Step 5: Install Ionic**

Next, you'll need to install Ionic. You can do this with the following command:

```
npm install @ionic/react
Or
npm install @ionic/react@6.0.0

```

**Step 6: Install Capacitor**

Now you can install Capacitor. First, you need to install the Capacitor CLI (Command Line Interface):

```
npm install @capacitor/cli @capacitor/core
```

After the Capacitor CLI is installed, you can add platforms (like iOS or Android) that you want your app to run on:

```
npx cap add ios
npx cap add android
```

You will also need to initialize Capacitor with your app information. Here's an example:

```
npx cap init myApp com.example.myapp
```

In the above command, `myApp` is the name of your app, and `com.example.myapp` is the bundle ID (generally in reverse-domain style).

**Step 7: Install additional dependencies**

Depending on the requirements of your project, you may need to install additional dependencies, such as React Router for navigation or Axios for HTTP requests.

With these installations, you should be ready to start building your app with Vite, React, Ionic, and Capacitor. Remember, you should always check the official documentation for these tools if you run into issues or need more detailed information.


<h1>Removing Packages Example:</h1>
If you want to remove a package that has already been installed, you can use the `npm uninstall` command followed by the package name. In your case, you can remove the version 7 of @ionic/react using the following command:

```bash

npm uninstall @ionic/react
Or
npm install react-router-dom@6.6.1

```

After running this command, the @ionic/react package will be removed from your node_modules directory, and its entry in the dependencies section of your package.json file will also be removed.

After uninstalling, you can install the specific version of the package you need (version 6.0.0 in your case) using the command I provided in the previous message.

Remember, each time you add or remove a package, it's a good idea to delete your `package-lock.json` file and `node_modules` folder and then run `npm install` to ensure all dependencies are correctly installed.

<h1> Installing React Router Dom V6 </h1>
To install `react-router-dom` at a specific version, you can specify the version number just like we did earlier with Ionic. 

Here is the command to install `react-router-dom` version 6.6.1:

```bash
npm install react-router-dom@6.6.1
```

This command will add `react-router-dom` version 6.6.1 to your `node_modules` folder and add an entry to the dependencies section of your `package.json` file.

After the installation process, you can confirm the installed version by using the `npm list` command:

```bash
npm list react-router-dom
```

This command will display the installed version of `react-router-dom` in your project. If everything went well, it should show version 6.6.1.


<h1>Adding Android and Ios Native Platforms</h1>
To install both `@capacitor/android` and `@capacitor/ios`, you need to run the following commands in your terminal:

1. Navigate to the root directory of your project:

```bash
cd /path/to/your/project
```

2. Install `@capacitor/android`:

```bash
npm install @capacitor/android
or
npm install @capacitor/android@5.0.4

```

3. Install `@capacitor/ios`:

```bash
npm install @capacitor/ios
or
npm install @capacitor/ios@5.0.4

```

You need to ensure that you have Node.js and npm installed in your development environment to use these commands. After installation, these packages will be added to your project's `node_modules` directory, and they will be listed in your `package.json` file under the "dependencies" section.

Remember to run `npx cap sync` after installing new plugins. This command updates each of your native platform projects so they have the latest assets and configuration data. This way, when you run `npx cap open android` or `npx cap open ios`, your IDE will be up-to-date.

