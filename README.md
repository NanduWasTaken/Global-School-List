# 🚀 Global School List  
---

> [!WARNING]
> **These lists were collected manually!**  GitHub does not allow automated scraping of our primary source: [GitHub Education](https://education.github.com) it is against their terms of service, so all the information in this repository was gathered through manual research.

> [!NOTE]
> This does not contain every school in the world, it only has 22000+ schools. We hope to add more schools in the furture.

## 📚 About This Repository  
This repository contains a list of **Educational Institutions**. There are over **22000+ unique institutions** in this list. The dataset includes:  
- 📌 School names  
- 🌐 Verified domains  
- ✅ Other Details

## 🔍 Why This Matters  
There no Open Source Database in the world containing every school name and details in the world. So i though I should contribute a little

## 📂 Available Files  

### **1️⃣ `json/fullSchoolList.json`**  
✅ **Purpose:** This is the **master database** containing all school details.  
✅ **Why Needed?**  
- Stores complete details of each school.  
- Used as the **source file** for generating the name-only lists.  
- Maintains structured information for future enhancements.  

📥 **[Download fullSchoolList.json](json/fullSchoolList.json)**  

#### **Example Structure:**
```json
[
  {
    "name": "University of Cambodia",
    "verification_required": false,
    "informal_partner": false,
    "allowlisted_domains": [],
    "other_domains": [],
    "issues_coupons": false,
    "school_system_present": false,
    "school_system_verification_required": null,
    "school_system_domains": null,
    "user_has_matching_email": false,
    "title": "University of Cambodia\n    (https://uc.edu.kh)\n    (សាកលវិទ្យាល័យកម្ពុជា)\n    (UC)"
  },
]
```

---

### **2️⃣ `json/schoolList.json`**  
✅ **Purpose:** This file **only contains school names** extracted from `fullSchoolList.json`.  
✅ **Why Needed?**  
- Useful for scripts or applications that only need the list of school names.  
- Helps in quickly checking whether a school is included in the database.  

📥 **[Download schoolList.json](json/schoolList.json)**  

#### **Example Structure:**
```json
[
  "Harvard University",
  "Stanford University"
]
```

---

### **3️⃣ `text/schoolList.txt`**  
✅ **Purpose:** This file contains the same school names as `schoolList.json`, but in **plain text format** with one name per line.  
✅ **Why Needed?**  
- Easily readable by humans and can be opened in any text editor.  
- Useful for quick lookups, copying, or pasting elsewhere.  

📥 **[Download schoolList.txt](text/schoolList.txt)**  

#### **Example Content:**
```
Harvard University
Stanford University
```

## 💪 How These Files Work Together  
1. **New schools are added** to `json/fullSchoolList.json`.  
2. **GitHub Actions workflow** automatically:  
   - Sorts the list alphabetically.  
   - Removes duplicate entries.  
   - Extracts school names to generate `json/schoolList.json` and `text/schoolList.txt`.  
   - Commits the updated files back to the repository.  

## 📥 Contributing  
If you find any incorrect or missing information, feel free to **open an issue** or **submit a pull request**!  

## 📜 License  
This project is open-source under the **MIT License**.  


## 📝 Disclaimer  
- This list is not 100% complete!
- This data is **not official** and is not 100% accurate and reliable.

## 📥 Contributing  
- If you find any incorrect or missing information, feel free to **open an issue** or **submit a pull request**!  
- Only add new Entries to the [Full Student List](https://github.com/NanduWasTaken/GitHub-Student-Program-School-List/blob/main/json/fullSchoolList.json) since there is a workflow to add the institution names to the rest of the files.

## 📜 License  
This project is open-source under the **MIT License**.  
