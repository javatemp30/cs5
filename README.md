# Program 5 — File Comparison for Forensic Investigation

## Aim
To compare two text files using **Compare It!** on Windows, identify modifications, and document the differences for a basic digital forensic investigation.

## Requirements
- Windows computer
- Notepad (or another plain-text editor)
- Compare It! file comparison application
- Two sample text files (`File1.txt` and `File2.txt`)

> This experiment is performed on **Windows**, not inside Kali Linux or VirtualBox.

## 1. Install Compare It!
1. Open a browser on Windows.
2. Visit the developer's website: https://www.grigsoft.com/wincmp3.htm
3. Find the Compare It! download, download the installer, and follow its setup instructions.
4. Launch **Compare It!** from the Start menu.

> Menus and icons can differ by software version.

## 2. Create the First File
1. Open **Notepad**.
2. Enter the following text:

```text
Student Name: Rahul
USN: 1DS22CS001
Department: CSE
Semester: 7
College: DSCE
```

3. Choose **File → Save As**.
4. Select **Desktop**, enter `File1.txt`, and save it. If needed, select **All files** to avoid creating `File1.txt.txt`.

## 3. Create the Second File
1. Open a new Notepad window.
2. Enter:

```text
Student Name: Rahul Kumar
USN: 1DS22CS001
Department: Computer Science
Semester: 7
College: DSCE Bangalore
```

3. Save it on the **Desktop** as `File2.txt`.

## 4. Load Both Files into Compare It!
1. Open **Compare It!**.
2. Use its file selection/open controls to load `File1.txt` into the left comparison pane.
3. Load `File2.txt` into the right comparison pane.
4. Start the comparison if it does not run automatically.
5. Confirm that both files appear side by side.

## 5. Examine the Differences
Compare It! highlights differences; highlight colors vary by version and settings.

| Field | File1.txt | File2.txt | Observation |
|---|---|---|---|
| Student Name | Rahul | Rahul Kumar | Modified |
| USN | 1DS22CS001 | 1DS22CS001 | Unchanged |
| Department | CSE | Computer Science | Modified |
| Semester | 7 | 7 | Unchanged |
| College | DSCE | DSCE Bangalore | Modified |

**Expected observation:** Three lines differ; two lines are unchanged.

## 6. Navigate the Changes
1. Locate **Next Difference** and **Previous Difference** on the toolbar or menus.
2. Move through each changed line.
3. Confirm that the highlighted text corresponds to the table above.

## 7. Document the Comparison
1. Look for **File → Print Preview** or **Print**, if available in your installed version.
2. If permitted, choose **Microsoft Print to PDF** and save a copy as `File_Comparison_Report.pdf`.
3. If the unregistered version restricts printing to one page, close the notice. You do **not** need to buy a license for this practice exercise.
4. Instead, capture the side-by-side comparison with **Win + Shift + S**, then save it as `File_Comparison.png`.
5. For a PDF submission, insert the screenshot into a Word document and export it to PDF.

> A screenshot records the visible comparison. It is not a substitute for a cryptographic integrity check or a full forensic audit trail.
