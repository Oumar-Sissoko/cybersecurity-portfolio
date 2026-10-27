# M57 Data Leak Investigation

**Scenario:** A confidential employee salary spreadsheet from M57.biz appeared on a competitor's website. I examined a disk image of the CFO's laptop to find when the file was created, how it left the company, and who was involved.

**Tools:** Autopsy (The Sleuth Kit) — metadata extraction, email parsing, keyword search, web and USB artifact review

**Key findings**
- File metadata showed the spreadsheet was authored by the company president and last saved by the CFO on July 19, 2008.
- Recovered emails showed the president requested employee names, salaries, and SSNs under a false pretext.
- Identified `alex@m57.biz` as a second account operated by the president, used to direct the file.
- No evidence the CFO distributed the file beyond the requested internal email.

**Conclusion:** Evidence points to the president as the source of the leak. Confirming the final upload would require examining her devices and mail server logs.

**Skills shown:** timeline reconstruction, metadata analysis, email artifact analysis, insider-threat investigation, evidence-based reporting
