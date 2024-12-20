# Installing Python and Pycharm were installed.

---
### Pycharm installation:
       ┌─────────────────────────────────┐
       │         Installation Guide      │
       └─────────────────────────────────┘

1. **Install JetBrains Products**
   - Download and install your desired JetBrains product.

2. **Download Crack**
   - Obtain the `ja-netfilter` crack files.

3. **For Windows:**
   - Copy the folder `ja-netfilter` to **Drive C:**.

4. **Auto-Configure vmoptions**  
   - **Windows:**
     - Execute one of the following scripts:
       - For the current user:  
         `scripts\install-current-user.vbs`
       - For all users:  
         `scripts\install-all-users.vbs`
   - **macOS/Linux:**
     - Run the following command:  
       `scripts/install.sh`

5. **Manual Configuration (Optional)**  
   - Locate the `*.exe.vmoptions` file in your JetBrains installation directory (e.g., `C:\Program Files\JetBrains\PhpStorm 2022.3\bin`).  
   - Open the file in a text editor like Notepad++ and append the following lines to the end of the file:

     **Windows:**
     ```
     -javaagent:C:\ja-netfilter\ja-netfilter.jar=jetbrains
     --add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
     --add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
     ```

     **macOS:**
     ```
     -javaagent:/Users/x/ja-netfilter/ja-netfilter.jar=jetbrains
     --add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
     --add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
     ```

     **Linux:**
     ```
     -javaagent:/home/x/ja-netfilter/ja-netfilter.jar=jetbrains
     --add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
     --add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
     ```

     *(Replace `x` with your username.)*

6. **Activate JetBrains Product**
   - **Option 1:** Use a license server and activate at:  
     `https://jetbra.in`
   - **Option 2:** Copy and paste the provided activation code into the "Activation Code" field.
