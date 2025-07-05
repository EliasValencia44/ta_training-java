# 🧪 Automated Test Framework

This project was developed to automate the **login functionality** of the website: [https://www.saucedemo.com/](https://www.saucedemo.com/).

The main goal is to validate the system's behavior under different login scenarios, ensuring the quality and stability of the site.

By default, the project runs the **3 test cases in parallel** to speed up execution.  
If you wish to modify this behavior, you can edit the configuration in the `junit-platform.properties` file.

## ✅ Test Cases Included

The framework currently covers **3 test cases**:

1. 🟢 Successful login with valid credentials.
2. 🔴 Failed login with invalid credentials.
3. ⚠️ Failed login with empty fields.

Each scenario is automated and can be executed on multiple supported browsers.


## 🚀 How to Run the Project

You can run the tests using the following command in your terminal:

```bash
mvn test -Dbrowser="browser_name"
```

### 🔧 Supported Browsers:

- `chrome` (default)
- `edge`
- `safari`
- `explorer`

> If no browser is specified, **Chrome** will be used by default.

### 🧾 Execution Example:

```bash
mvn test -Dbrowser="chrome"
```

or simply:

```bash
mvn test
```

## 📊 Generating Reports

To run the tests and generate reports, use the following command:

```bash
mvn test -Dbrowser="chrome" site
```

The reports will be automatically generated in the `target/site` directory.
