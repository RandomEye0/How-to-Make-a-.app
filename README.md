
---

## 🛠️ **Compiling the Application**

Now that we've set up everything, let's compile the app.

1. **Navigate to the `MacOS` folder** where the `main.mm` file is located:

    ```bash
    cd ~/Desktop/YourAppName.app/Contents/MacOS
    ```

2. **Compile the `main.mm` file** using `clang++`:

    ```bash
    clang++ -o YourAppNameExecutable -framework Cocoa main.mm
    ```

    - **Explanation**:
      - This command compiles your `main.mm` file and links it with the **Cocoa framework** to handle the graphical interface.
      - The compiled output will be saved as `YourAppNameExecutable`.

---

## 🎨 **Customization**

You can easily customize the application by editing the following:

- **Window Size**: Change the `NSMakeRect(0, 0, 480, 320)` values to adjust the size of the window.
- **Window Title**: Modify `[window setTitle:@"YourAppName"];` with the title you prefer.
- **Displayed Text**: Change `[label setStringValue:@"Your Custom Text Here"];` to display your custom message.

---

## 🐛 **Troubleshooting**

- **App Not Opening?**: Make sure you've set the correct file permissions. Run this command to ensure your app is executable:

    ```bash
    chmod +x ~/Desktop/YourAppName.app/Contents/MacOS/YourAppNameExecutable
    ```

- **Missing `.dylib` or Dependencies?**: Ensure all required libraries and files are properly linked in your app's structure.

---

## 🤝 **Contributing**

If you find any issues or want to improve the project, feel free to fork the repository and submit a pull request! Any contributions are welcome.

---

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### **Conclusion**

You’ve now successfully created a **macOS `.app` file** that displays custom text in a window! 🎉 You can easily modify the code to display different content, add more functionality, or build it out into a full-fledged macOS app.

Let me know if you run into any issues or need additional help! 😊
