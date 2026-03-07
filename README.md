# AgilerRefactoring
AgilerRefactoring is an experimental extension that supports refactoring and code generation for the GeneXus IDE.  
It helps developers refactor existing code and generate procedures based on Transaction objects to improve productivity.

---
# Features
AgilerRefactoring provides the following main functions:

| Feature | Description |
|---|---|
| 🔍 Source Review | Review and fix GeneXus source code based on basic coding rules. |
| ⚙️ Updater Generator | Generate an updater procedure using Business Components (BC). |
| ⚙️ Updater Generator (FE) | Generate an updater procedure using `For Each`. |
| 📥 Retriever Generator | Generate a retrieval procedure using `For Each`. |
| 🧪 Trace Model Generator | Under development (T.B.D). |

---

# Requirements
GeneXus 18 U12 is tested.

---

# Download
The stable version is distributed via the GeneXus Marketplace.

---

# Installation
1. First, create the folder `C:\temp`.  
   (Log files are generated in this folder by default.)

2. Download the AgilerRefactoring zip file from the GeneXus Marketplace.

3. Extract the zip file and copy the following four files to the specified locations.

| File | Destination Folder | Example Path |
|-----|-----|-----|
| Agiler.Refactorings.Common.dll | Install folder | C:\Program Files (x86)\GeneXus\GeneXus18 |
| Newtonsoft.Json.dll | Packages folder | C:\Program Files (x86)\GeneXus\GeneXus18\Packages |
| Agiler.Packages.Refactorings.BL.dll | Packages folder | C:\Program Files (x86)\GeneXus\GeneXus18\Packages |
| Agiler.Packages.Refactorings.UI.dll | Packages folder | C:\Program Files (x86)\GeneXus\GeneXus18\Packages |

4. Open a command prompt, move to the GeneXus installation folder, and execute the following command: genexus.exe /install

5. Start GeneXus.

Example:
cd "C:\Program Files (x86)\GeneXus\GeneXus18"
genexus.exe /install
genexus.exe 

---

# Uninstallation

Delete the following files from the corresponding folders.

| File | Folder |Example Path |
|-----|-----|-----|
| Agiler.Refactorings.Common.dll | GeneXus Install folder |C:\Program Files (x86)\GeneXus\GeneXus18 |
| Newtonsoft.Json.dll | Packages folder |C:\Program Files (x86)\GeneXus\GeneXus18\Packages |
| Agiler.Packages.Refactorings.BL.dll | Packages folder |C:\Program Files (x86)\GeneXus\GeneXus18\Packages |
| Agiler.Packages.Refactorings.UI.dll | Packages folder |C:\Program Files (x86)\GeneXus\GeneXus18\Packages |


3. Open a command prompt, move to the GeneXus installation folder, and run: genexus.exe /install


Example:
cd "C:\Program Files (x86)\GeneXus\GeneXus18"
genexus.exe /install

---

# FAQ

### Q: Can I change the automatically generated Japanese header to an English header?

A: Yes. Please customize the `HeaderTemplate` in the following configuration file located in the model folder:

Example:


C:\Models\KB_Name_\AgilerRefactoringsSettings.json


---

# Author

Miura Masayuki  
System Development LLC

---

# Architecture

Extension based on the GeneXus Platform SDK.

---

# Disclaimer

This software is provided **"as is"**, without warranty of any kind.  
Use at your own risk.

---

# License and Terms of Use

- AgilerRefactoring is an experimental project.
- The developer and distributor assume no responsibility for any damages or issues arising from its use.
- This software is provided without any warranty.

Details:

https://agiler.jp/TermsOfProduct.html

- Third-party libraries used in this software are subject to their respective licenses.

---

# Third-Party Libraries

This software includes the following third-party library:

### Newtonsoft.Json

Copyright (c) James Newton-King  
Licensed under the MIT License.

Newtonsoft.Json is used for JSON serialization and deserialization.

Project website  
https://www.newtonsoft.com/json

---
# AgilerRefactoring Project Website (Japanese)
https://agiler.jp/labs/AgilerRefactoring

License  
https://github.com/JamesNK/Newtonsoft.Json/blob/master/LICENSE.md
