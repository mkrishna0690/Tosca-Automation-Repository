# Tosca-Automation-Repository
Tosca Automating 

#1 --  **TCP (Test Configuration Paramter):** It is mainly used to store the test data.If you want you can use that test data where ever required. 

**Purpose of TCP:** 
          Maintenace of data is very easy and 
          Reusability of data 
          
**Syntax:**  {CP[TCP_Name]}

**How to create TCP:**  Right Click on Testcase and select **‘Create TCP’ {purple color ICON}**

     

#2 -- **Cross-browser testing OR Multi-browser testing:**
            Perform testing on same functionality in different browsers then it is called Cross-browser testing.

     

#3 -- **Re-Scan:** It is mainly used to update the exisiting user defined modules.


#4 -- **Various ACTION MODES:** This will apply to step level only.

         - In details view, you'll see ActionMode.
         - Default ActionMode is **Input**

  *** **Verify** ActionMode: It is used to verify the control's
                             a.Exists or Not
                             b.Enabled or Not
                             c.Visible or Not 
                             d.Innertext
                

 #5 **Waiting Methods in TOSCA**:

       - TBox wait (static wait time)
       - Synchronization Timeout: It is TOSCA's default wait time (dynamic wait)
                                  1.Tosca’s default wait time - 10 secs (10000 milliseconds)  
                                  2.Location: Project > settings > TBox > Synchronization.

       - Synchronization timeout during WAITON: 
                                 1.Default wait time - 20 secs (20000 milliseconds)
                                 2.It applies to particular step where the ActionMode is WaitON
 


   #5 **How to take a screenshots in TOSCA?**

        In 2 ways, you can take the screenshots

        1.**TBox Take Screenshot (Standard module):** 
        
                 Click on    **TBox Automation Tools > Basic Windows Operations > TBox Take Screenshot**
                 

        2.**Doku snapper (Tool feature):**
        
           Path to find Doku Snapper: Project > Settings > Engine > DokuSnapper
             
