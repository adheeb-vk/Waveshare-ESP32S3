# ESP32-S3 with 7-inch Display  

## 🌟 UI for Waveshare  

This project demonstrates how to create a user interface (UI) for the **Waveshare ESP32-S3 7-inch Display** using the **LVGL (Light and Versatile Graphics Library)**. Designing UI elements with LVGL can be challenging, so we simplify the process using **SquareLine Studio**, a drag-and-drop interface that converts designs into LVGL format.  

For programming the board, we utilize **ESP-IDE (Espressif IDE)**, a comprehensive development environment provided by Espressif.  

---

## 🚀 Getting Started  

### 🛠️ **Required Tools and Resources**  

- **SquareLine Studio**: [Download here](https://squareline.io/downloads#lastRelease)  
- **Espressif IDE**: [Download the appropriate version](https://dl.espressif.com/dl/esp-idf)

  ![Screenshot 2024-11-08 111219](https://github.com/user-attachments/assets/ff9b31bc-9137-4ab6-ac6c-1a9e25c8adb6)


---

## 🖌️ Creating the UI  

1. **Add Waveshare Board Extension**  
   To get started, you'll need to add an extension for the Waveshare board in SquareLine Studio.  
   Download the extension from this repository:  
   [Waveshare Extension Repository](https://github.com/adheeb-vk/Waveshare-ESP32S3/).  

   **Steps to Install the Extension**:  
   1. Open the `SquareLine` folder in your file system:  
      - Navigate to `C:\Users\<Your Username>\SquareLine\boards\Espressif`.  
   2. Paste the downloaded **Waveshare folder** into the directory.  

2. **Create UI in SquareLine Studio**  
   - Open SquareLine Studio and select the **Create** option.  
   - Choose **Espressif**, and you'll see the Waveshare board option.  
   - Use the drag-and-drop tools on the left to design your UI.  
   - Edit properties of UI elements on the right.  
   - For simplicity, we’ll use a minimal UI with a single button.  

   **Saving the Project**:  
   - After finishing your UI design, click **Create Template Project** and save it in your desired directory.  

---

## 💻 Programming the Board  

1. **Create a New ESP-IDF Project**  
   - Open ESP-IDE and right-click in the project explorer.  
   - Select `New > Espressif IDF Project`.  
   - Enter a project name and choose the **ESP32-S3** board.  

2. **Import SquareLine Studio Files**  
   - Right-click the project folder and select **Import**.  
   - In the pop-up window, choose **File System** under the General folder.  
   - Browse to the SquareLine Studio project folder you created earlier.  
   - Check the **Overwrite existing resources without warning** option and click **Finish**.  

3. **Adjust `sdkconfig`**  
   - Locate and double-click the `sdkconfig` file in the project folder.  
   - Navigate to **LVGL Configuration**.  
   - Disable **Custom Fonts** and **Lottie Library** if they’re not in use.  

---

## ⚙️ Building and Flashing  

1. **Build the Project**  
   - Click the hammer icon in ESP-IDE to build the project. (This may take some time.)  

2. **Set the COM Port**  
   - Click the settings icon next to the board name and configure your **COM port**.  

3. **Flash the Firmware**  
   - Once the build is complete, flash the firmware to the board.  

You should now see your custom-designed UI displayed on the Waveshare 7-inch touch screen!  

---

## 🎉 Happy Hacking!  

Feel free to reach out or open an issue if you need any assistance with the setup. Contributions are welcome to improve this project further.  

---

