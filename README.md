# Oracle PDB Assignment II

**Student Name:** Justin MICOMYIZA
**Student ID:** 29403
**Course:** Oracle Database
**Assignment:** Assignment II – Oracle Pluggable Database (PDB)

## 1. Overview

This assignment demonstrates the creation, management, and deletion of Oracle Pluggable Databases (PDBs), as well as the use of Oracle Enterprise Manager (OEM).

The assignment consists of four mandatory tasks:

1. Create a new Pluggable Database
2. Create and delete a temporary Pluggable Database
3. Access Oracle Enterprise Manager
4. Document and report the completed work on GitHub

## 2. Oracle Environment

* **Database:** Oracle Database 21c
* **Database Name:** ORCL21
* **Tool Used:** Oracle SQL Developer
* **Operating System:** Windows
* **PDB Created:** `JU_PDB_29403`
* **PDB User:** `JUSTIN_PLSQLAUCA_29403`

## 3. Task 1 — Create a New Pluggable Database

A new Pluggable Database named `JU_PDB_29403` was created according to the required naming convention.

The PDB was successfully opened and verified with `READ WRITE` status.

The required user account `JUSTIN_PLSQLAUCA_29403` was also created inside the PDB and given the necessary privileges for future class work.

### Evidence

The screenshots for PDB creation and verification are available in:

`![Create PDB](create pdb.png)`

## 4. Task 2 — Create and Delete a PDB

A temporary PDB named:

`JU_TO_DELETE_PDB_29403`

was created successfully.

Its existence was verified before it was completely removed using the `INCLUDING DATAFILES` option.

The PDB was then checked again to confirm that it no longer existed.

### Evidence

The screenshots for temporary PDB creation and deletion are available in:

`![PDB to Delete](pdb to delete.png)`

## 5. Task 3 — Oracle Enterprise Manager

Oracle Enterprise Manager Express was accessed successfully through the configured HTTPS port.

The Oracle environment was displayed through the Enterprise Manager dashboard.

### Evidence

The OEM dashboard screenshot is available in:

`![OEM](oem.png)`

## 6. Challenges Faced and Solutions

### Challenge 1: FILE_NAME_CONVERT Error

During PDB creation, Oracle returned `ORA-65016`, indicating that `FILE_NAME_CONVERT` needed to be specified.

**Solution:** The Oracle datafile location was identified and the `FILE_NAME_CONVERT` clause was included when creating the PDB.

### Challenge 2: Insufficient Privileges

An `ORA-01031` error occurred when attempting to open the PDB while connected as the `SYSTEM` user.

**Solution:** A SQL Developer connection using `SYS` with the `SYSDBA` role was created and used for the required administrative operation.

### Challenge 3: PDB User Verification

The required class user was initially not present in the PDB.

**Solution:** The session was changed to `JU_PDB_29403`, after which the required user `JUSTIN_PLSQLAUCA_29403` was created and granted the required privileges.

## 7. Integrity Statement

I confirm that the work presented in this repository represents my work completed for this assignment. The screenshots and documentation provide evidence of the Oracle PDB operations and Oracle Enterprise Manager setup performed during the assignment.

## 8. Submission Details

**Repository Link:**
https://github.com/justinmicomyiza6-cmyk/oracle_pdb_ass_II_29403_justin

**PDB Name Created:**
`JU_PDB_29403`

**Issues Encountered:**
Yes

**Student Name:**
Justin MICOMYIZA

**Student ID:**
29403
