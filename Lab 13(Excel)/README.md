# 📘 Grade Sheet – First Terminal Exam (Class 11 - Management)

---

## 🏫 Institution:
**Milestone International Secondary School**

## 🧪 Examination:
**First Terminal Examination – Academic Year 2078 (B.S.)**

## 🧑‍🏫 Faculty:
**Management Stream – Grade 11**

---

## 📂 File Purpose:

This Excel workbook is designed to **record, calculate, analyze, and report** student academic performance during the First Terminal Examination for Class 11 (Management).

The file:

- Stores individual subject marks  
- Automatically computes totals, percentages, grades, and GPA  
- Highlights student performance with letter grades and grade points  
- Applies pass/fail criteria based on subject-wise minimum marks  
- Uses subject weightings to calculate GPA fairly  

---

## 📊 Contents of the Grade Sheet:

Each **row** (from row 4 onward) represents one student.  
Each **column** holds specific types of data:

| Column | Label   | Description |
|--------|---------|-------------|
| A      | RNo.    | Roll Number of the student |
| B      | Name    | Full name of the student |
| C–H    | Eng, Nep, Soc, Eco, Acc, CS | Marks obtained in individual subjects:<br>• Eng = English<br>• Nep = Nepali<br>• Soc = Social Studies<br>• Eco = Economics<br>• Acc = Accountancy<br>• CS = Computer Science |
| I      | Total   | Sum of marks across all 6 subjects |
| J      | %       | Overall percentage score |
| K      | Res     | Pass/Fail based on minimum subject-wise marks |
| L–Q    | EngG to CSG | Subject-wise letter grades |
| R–W    | EngGP to CSGP | Subject-wise grade points (numerical form of grades) |
| X      | GPA     | Final Grade Point Average based on subject weightage |

---

## 🧮 Grading Criteria (Letter Grades & Grade Points):

| Marks Range | Letter Grade | Grade Point |
|-------------|--------------|-------------|
| 68–75       | A+           | 4.0         |
| 60–67       | A            | 3.6         |
| 53–59       | B+           | 3.2         |
| 45–52       | B            | 2.8         |
| 37–44       | C+           | 2.4         |
| 30–36       | C            | 2.0         |
| 26–29       | D            | 1.6         |
| Below 26 (or <18 in CS) | NG (Not Graded) | NG |

---

## ✅ Pass/Fail Rule:

To be marked as **Pass**, a student must score:

| Subject           | Minimum Marks to Pass |
|------------------|------------------------|
| English, Nepali, Social, Economics, Accountancy | 26 |
| Computer Science  | 18 |

If **any one** subject falls below the minimum, the result will be **Fail**.

---

## 📐 Subject Weightings for GPA Calculation:

| Subject          | Weight |
|------------------|--------|
| English          | 3.00   |
| Nepali           | 2.25   |
| Social Studies   | 3.75   |
| Economics        | 3.75   |
| Accountancy      | 3.75   |
| Computer Science | 2.50   |

### 🧠 GPA Formula:

```excel
GPA = (EngGP*3 + NepGP*2.25 + SocGP*3.75 + EcoGP*3.75 + AccGP*3.75 + CSGP*2.5) / 19
```
In this formula, means subject * credit hours of the subject.

## 💡 Examples for Better Understanding

### 🎯 Example 1: High Performing Student

- **Name**: Bhushan Dahal  
- **Marks**:  
  - English: 60  
  - Nepali: 63  
  - Social Studies: 50  
  - Economics: 39  
  - Accountancy: 60  
  - Computer Science: 43  
- **Total**: 315  
- **Percentage**: 74.12%  
- **Result**: ✅ Pass  
- **GPA**: 3.21  
- **Grades**: Mostly A’s and B’s  

---

### ⚠️ Example 2: Just Passing

- **Name**: Ram Karki  
- **Marks**:  
  - English: 40  
  - Nepali: 48  
  - Social Studies: 30  
  - Economics: 56  
  - Accountancy: 30  
  - Computer Science: 34  
- **Total**: 238  
- **Percentage**: 56%  
- **Result**: ✅ Pass  
- **GPA**: 2.50  
- **Grades**: Mostly C’s  

---

## 🔧 Formulas Used in the File

### ➕ Total Marks:
```
=SUM(C4:H4)
```

### 📈  Percentage:
```
=I4/4.25
```

### 🛡️ Result (Pass/Fail Logic):
```
=IF(AND(C4>=26, D4>=26, E4>=26, F4>=26, G4>=26, H4>=18), "Pass", "Fail")
```

### 🔤 Grade Calculation (Example for English):
```
=IF(AND(C4>=68,C4<=75),"A+", IF(AND(C4>=60,C4<=67),"A", IF(AND(C4>=53,C4<=59),"B+", IF(AND(C4>=45,C4<=52),"B", IF(AND(C4>=37,C4<=44),"C+", IF(AND(C4>=30,C4<=36),"C", IF(AND(C4>=26,C4<=29),"D", "NG")))))))
```

### 🔢 Grade Point Calculation (Example for English):
```
=IF(AND(C4>=68,C4<=75),4.0, IF(AND(C4>=60,C4<=67),3.6, IF(AND(C4>=53,C4<=59),3.2, IF(AND(C4>=45,C4<=52),2.8, IF(AND(C4>=37,C4<=44),2.4, IF(AND(C4>=30,C4<=36),2.0, IF(AND(C4>=26,C4<=29),1.6, "NG")))))))
```

### 📊 GPA Calculation:
```
=(R4*3 + S4*2.25 + T4*3.75 + U4*3.75 + V4*3.75 + W4*2.5) / 19
```

## 👩‍🏫 Instructions for Use
- Input marks in columns C to H (English to Computer Science)
- Columns I to X will auto-calculate if formulas are present
- Use drag fill to extend formulas to new student rows
- Protect or lock columns with formulas to avoid accidental deletion
- When adding a new student, copy a full row with formulas
- Watch for conditional formatting (e.g., red for fail, green for top scorers)

## 📌 Recommendations
- ✅ Validate input data before sharing or analyzing
- 🔁 Keep a backup copy before any major updates
- 📘 Adjust grade boundaries and subject weightings based on curriculum changes
- 📊 Use Excel or Google Sheets charts for:
    - GPA trends
    - Subject-wise averages
    - Student comparison

## 🗃️ File Format
- File Type: .xlsx
- Software Compatibility:
    - Microsoft Excel (2016 or newer)
    - Google Sheets
    - LibreOffice Calc

## 🌟 Suggested Enhancements (Optional)
- 📈 GPA Distribution Chart
- 📑 Summary Dashboard
- 🧮 GPA-Based Class Ranking
- 🖨️ Printable Layouts for Student Reports
- 📤 Mail Merge for generating individual mark sheets with MS Word

## 📌 Usage Tips
- Enter only numeric values in the mark entry columns
- Do not edit grade/percentage/GPA formula cells unless necessary
- Use data validation tools to avoid invalid inputs
- Duplicate the sheet for future terms, exams, or academic years

## 🔁 Versioning
- Version: 1.0
- Release Date: 2078 B.S. (First Terminal Exam)
- Format: .xlsx
- Supported Platforms: Microsoft Excel, Google Sheets, LibreOffic

---

# 📋 Student Performance Summary (Sample Data)

Below is a summary of student performance from the First Terminal Examination of Class 11 (Management). This includes subject-wise marks, total score, percentage, GPA, and final result.

## 🧾 Table: Student Results (Sample of 10 Students)

| RNo. | Name            | Eng | Nep | Soc | Eco | Acc | CS | Total | %     | Result | GPA  |
|------|------------------|-----|-----|-----|-----|-----|----|--------|-------|--------|------|
| 1    | Ram Karki        | 40  | 48  | 30  | 56  | 30  | 34 | 238    | 56.00 | Pass   | 2.50 |
| 2    | Shyam Shah       | 45  | 45  | 34  | 45  | 35  | 25 | 229    | 53.88 | Pass   | 2.43 |
| 3    | Hari Khadka      | 47  | 60  | 38  | 58  | 36  | 28 | 267    | 62.82 | Pass   | 2.68 |
| 4    | Yubraj Humagai   | 50  | 50  | 40  | 48  | 40  | 30 | 258    | 60.71 | Pass   | 2.64 |
| 5    | Suraj Magar      | 42  | 55  | 39  | 49  | 38  | 25 | 248    | 58.35 | Pass   | 2.57 |
| 6    | Kushal Lama      | 55  | 59  | 45  | 35  | 55  | 40 | 289    | 68.00 | Pass   | 2.94 |
| 7    | Bhushan Dahal    | 60  | 63  | 50  | 39  | 60  | 43 | 315    | 74.12 | Pass   | 3.21 |
| 8    | Udit Shakya      | 41  | 53  | 38  | 43  | 42  | 33 | 250    | 58.82 | Pass   | 2.55 |
| 9    | Rajesh Tamang    | 49  | 58  | 47  | 46  | 47  | 27 | 274    | 64.47 | Pass   | 2.79 |
| 10   | Sohan Shrestha   | 57  | 41  | 31  | 40  | 34  | 30 | 233    | 54.82 | Pass   | 2.42 |

> 🎯 **Top Performer**: *Bhushan Dahal* with a GPA of **3.21** and total marks **315/425**
> 
> ⚠️ **Needs Improvement**: *Shyam Shah* and *Sohan Shrestha* have GPAs just above 2.40

---

## 📘 GPA Interpretation Guide:

| GPA Range | Interpretation         |
|-----------|-------------------------|
| 3.6 – 4.0 | Excellent               |
| 3.0 – 3.5 | Very Good               |
| 2.5 – 2.9 | Good                    |
| 2.0 – 2.4 | Satisfactory/Needs Support |
| < 2.0     | At Risk (Consider Remedial) |

---

