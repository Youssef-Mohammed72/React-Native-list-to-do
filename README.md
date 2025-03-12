# Task Manager App

## 📌 Overview
A simple **React Native Task Manager App** that allows users to add, complete, and remove tasks. This project is designed to enhance productivity by maintaining a task list.

## 🚀 Features
- Add new tasks to the list
- Mark tasks as completed by tapping on them
- Remove completed tasks from the list
- Responsive and user-friendly interface

## 🛠️ Tech Stack
- **React Native**
- **JavaScript**
- **Expo** (for testing and development)

## 📸 Screenshots
![image](https://github.com/user-attachments/assets/3684cc5e-def1-4bb4-ae01-7b0173546674)
![image](https://github.com/user-attachments/assets/53764fb9-224f-4890-a14f-226fa79da839)
![image](https://github.com/user-attachments/assets/4361c024-088d-4307-a370-3d2e4196f203)

## 🎨 UI Design
### Colors Used:
- **Background Color:** `#E8EAED` (Light Gray)
- **Task Background:** `#FFF` (White)
- **Task Indicator:** `#55BCF6` (Blue)

### Fonts:
- **Main Font:** Default React Native Font
- **Title Font Size:** `24px`, Bold
- **Task Font Size:** Default

## 📂 Project Structure
```
LIST-TO-DO/
│-- components/
│   ├── Task.js
│-- App.js
│-- package.json
│-- README.md
```

## 🏗️ Installation & Setup
### Prerequisites:
- Install **Node.js** & **npm**
- Install **Expo CLI** globally:
  ```sh
  npm install -g expo-cli
  ```

### Clone the Repository:
```sh
git clone https://github.com/Youssef-Mohammed72/React-Native-list-to-do.git
cd React-Native-list-to-do
```

### Install Dependencies:
```sh
npm install
```

### Run the App:
```sh
npm start
```
(Use Expo Go to scan the QR code and test the app on your mobile device.)

## 🟦 Run Online on Expo Snack

You can also test the app directly on Expo's online compiler:
[Run on Expo S](https://snack.expo.dev/@youssef_mohamed/to-do-list?platform=android)[nack](https://snack.expo.dev/@youssef_mohamed/to-do-list?platform=android)

## 📜 Code Highlights
### `App.js`
```javascript
const handleAddTask = () => {
  if (!task || task.trim().length === 0) return;
  Keyboard.dismiss();
  setTaskItems([...taskItems, task.trim()]);
  setTask('');
};
```

### `Task.js`
```javascript
const Task = (props) => {
    return (
        <View style={styles.item}>
            <Text style={styles.itemText}>{props.text}</Text>
        </View>
    );
}
```

## 📜 License
This project is **MIT Licensed**. Feel free to use and modify it as needed.

---
Made with ❤️ by [Youssef Mohammed](https://github.com/Youssef-Mohammed72)

