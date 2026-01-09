# First Mobile App 


###  Project Overview 
Mobile Application setup that provides provides a foundation for efficient mobile development with React Native and Expo.

### Objective: 
Setting up an Expo Router mobile application, customizing the home screen, testing on physical devices, and documenting the entire process including the reset-project command functionality.

### Step 1: Created the Project
```bash
# In my terminal:
cd prodev-mobile-setup
npx create-expo-app@latest .
```
 **What happened:** Created a fresh React Native app with Expo Router

### Step 2: Made It My Own
1. Opened `app/(tabs)/index.tsx`
2. Found this line:
```typescript
<Text>Welcome!</Text>
```
3. Changed it to:
```typescript
<Text>** First App Created**</Text>
```
**Result:** Now my app shows "** First App Created**" instead of "Welcome!"

### Step 3: Saw My App Live
```bash
npx expo start
```
**Cool part:** A QR code appeared in my terminal! I scanned it with my iPhone's camera and my app opened on my phone instantly!

## The Reset Experiment (What Actually Happened)

I ran the reset command to see what would happen:

```bash
npm run reset-project
```

**Here's what actually went down:**

```
Do you want to move existing files to /app-example instead of deleting them? (Y/n): y
```

I pressed `Y` (This means it's saves my work!)

**The reset did this:**
1. Created `/app-example` folder
2. Moved all my existing files there (saved my "** First App Created**" change!)
3. Created fresh `/app` folder with basic files
4. Gave me clear next steps

**What I learned:** The reset doesn't delete my work, it archives it and gives me a clean slate!


### Minor Hiccup I Encountered:
```
Unable to run simctl:
Error: xcrun simctl help exited with non-zero code: 72
```
**No big deal!** This just means my computer doesn't have iOS simulator set up. The app still works perfectly on my actual iPhone via QR code.

## My Project Structure (After Everything)

Here's what my folder looks like now:

```
prodev-mobile-app-0x00/
├── app/                    ← FRESH START (created by reset)
│   ├── index.tsx         ← New main file to edit
│   └── _layout.tsx       ← New layout file
├── app-example/          ← MY OLD WORK (saved here!)
│   ├── app/
│   │   └── (tabs)/
│   │       └── index.tsx ← My "** First App Created**" change is here!
│   ├── components/
│   ├── hooks/
│   ├── constants/        ← Colors.tsx file
│   └── scripts/          ← Reset script that I used
├── assets/
├── node_modules/
└── package.json
```

## Simple Commands I Used

### 1. Start Development:
```bash
npx expo start
```
**What happens:** Shows QR code → Scan with phone → App opens!

### 2. Reset Project (When Needed):
```bash
npm run reset-project
```
**Protip:** Always press `Y` when asked about moving files - it saves your work!

### 3. Stop the Server:
Press `Ctrl + C` in terminal

## Real Tips From My Experience

### Do This First Time:
1. **Use physical phone** - QR code scanning is magic
2. **Keep Wi-Fi on** - Phone and computer need same network


### If Something Goes Wrong:
1. **Close and restart** `npx expo start`
2. **Clear cache:** `npx expo start --clear`
3. **Check Wi-Fi** - Most issues are network-related

## My Actual Code Changes

### What I Modified (in app-example):
**File:** `app-example/app/(tabs)/index.tsx`
```typescript
// BEFORE:
<Text>Welcome!</Text>

// AFTER MY CHANGE:
<Text>** First App Created**</Text>
```

### What's in Colors.tsx:
**File:** `app-example/constants/Colors.tsx`
Contains color definitions for light/dark modes - useful for theming!

## What I Successfully Accomplished

1. **Created** my first Expo app
2. **Customized** the home screen text
3. **Ran** it on my actual iPhone
4. **Tested** the reset command (safely!)
5. **Documented** everything as I went
