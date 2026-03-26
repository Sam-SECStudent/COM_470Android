# COM_470Android
This wiki will cover the version history of an App created for the class
3/26/2026
# 📱 Vice‑Tracking Android App  
### *Software Development Life Cycle (SDLC) Outline*

## 1. **Planning**
The goal of this project is to develop an Android application that helps users track their progress in staying off a chosen vice (e.g., alcohol, drugs, nicotine).  

**Objectives**
- Provide a simple, supportive tool for daily accountability  
- Track streaks and progress over time  
- Offer optional reminders and motivational messaging  
- Ensure the app works offline and stores data securely  

**Core Features**
- Daily check‑in system  
- Streak calculation and display  
- History view (list or calendar)  
- Optional notifications  
- Local data storage  

**Constraints**
- Semester timeline  
- Android development skill level  
- Device compatibility  

## 2. **Requirements Analysis**

### **Functional Requirements**
- User selects a vice to track  
- User logs daily progress  
- App calculates streaks automatically  
- App displays history of entries  
- App sends optional reminders  
- App stores data locally  

### **Non‑Functional Requirements**
- Clean, intuitive UI  
- Fast load time  
- Offline functionality  
- Secure data handling  

## 3. **System & Architecture Design**

### **Architecture**
- **MVVM (Model‑View‑ViewModel)** for clean separation of concerns  
- **Jetpack Navigation** for screen transitions  
- **Room Database** for persistent local storage  

### **Key Components**
- **Activities:** Onboarding, Dashboard  
- **Fragments:** Daily Check‑In, History View  
- **ViewModels:** Streak logic, entry management  
- **PendingIntent + AlarmManager:** Reminder notifications  
- **SharedPreferences:** User settings  

### **Data Models**
- `UserVice`  
- `DailyEntry`  
- `StreakRecord`  

## 4. **Implementation**

### **Development Tasks**
- Build UI layouts using XML + Jetpack components  
- Implement Room entities, DAO, and database  
- Create ViewModels for business logic  
- Add notification scheduling  
- Implement navigation graph  
- Test on emulator and physical device  

## 5. **Testing**

### **Unit Tests**
- Streak calculation  
- Date handling  
- Database CRUD operations  

### **UI Tests**
- Navigation flow  
- Input validation  
- Error handling  

### **Integration Tests**
- Notification triggers  
- Data persistence across restarts  

### **User Acceptance Testing**
- Validate ease of use  
- Confirm motivational flow and clarity  

## 6. **Deployment**
- Build release APK  
- Optimize performance and size  
- Prepare documentation  
- Submit for academic evaluation or internal testing  

## 7. **Maintenance**
- Fix bugs and refine UI  
- Improve performance  
- Add enhancements such as:
  - Charts and analytics  
  - Widgets  
  - Cloud sync  
  - Social accountability features  
