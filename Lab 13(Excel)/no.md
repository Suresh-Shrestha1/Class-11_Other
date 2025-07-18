📈 Percentage Calculation
=I4/4.25

Purpose: Calculates the percentage of the total score.

Explanation: Divides the total marks in cell I4 by the maximum possible marks (4.25), converting the result into a percentage score.

🛡️ Result (Pass/Fail Logic)
=IF(AND(C4>=26, D4>=26, E4>=26, F4>=26, G4>=26, H4>=18), "Pass", "Fail")

Purpose: Determines whether a student has passed or failed.

Explanation: The student passes only if they score at least 26 marks in subjects C4 to G4, and at least 18 in H4. Otherwise, they fail.

🔤 Grade Calculation (Example for English)
excel
Copy
Edit
=IF(AND(C4>=68,C4<=75),"A+", 
 IF(AND(C4>=60,C4<=67),"A", 
 IF(AND(C4>=53,C4<=59),"B+", 
 IF(AND(C4>=45,C4<=52),"B", 
 IF(AND(C4>=37,C4<=44),"C+", 
 IF(AND(C4>=30,C4<=36),"C", 
 IF(AND(C4>=26,C4<=29),"D", 
 "NG")))))))
Purpose: Assigns a letter grade based on marks in English.

Explanation: Evaluates the marks in C4 and assigns a grade from A+ to D, or NG (No Grade) if below 26.

🔢 Grade Point Calculation (Example for English)
excel
Copy
Edit
=IF(AND(C4>=68,C4<=75),4.0, 
 IF(AND(C4>=60,C4<=67),3.6, 
 IF(AND(C4>=53,C4<=59),3.2, 
 IF(AND(C4>=45,C4<=52),2.8, 
 IF(AND(C4>=37,C4<=44),2.4, 
 IF(AND(C4>=30,C4<=36),2.0, 
 IF(AND(C4>=26,C4<=29),1.6, 
 "NG")))))))
Purpose: Converts marks into grade points for GPA calculation.

Explanation: Uses the marks in English (C4) to assign a numerical grade point from 4.0 to 1.6, or "NG" if the student has not passed.

📊 GPA Calculation
=(R4*3 + S4*2.25 + T4*3.75 + U4*3.75 + V4*3.75 + W4*2.5) / 19

Purpose: Calculates the overall GPA based on weighted grade points.

Explanation: Multiplies each subject’s grade point (from R4 to W4) by its respective credit hours, adds them, and divides the total by 19 (sum of credit hours) to get the weighted average GPA.
