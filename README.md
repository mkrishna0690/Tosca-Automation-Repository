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
 


   #6 **How to take a screenshots in TOSCA?**

        In 2 ways, you can take the screenshots

        1.TBox Take Screenshot (Standard module):
        
                 Click on    **TBox Automation Tools > Basic Windows Operations > TBox Take Screenshot**
                 

        2.Doku snapper (Tool feature):
        
           Path to find Doku Snapper: Project > Settings > Engine > DokuSnapper


    #7 **BUFFERS:** In TOSCA, you've 2 types of Buffers

            1.Static Buffer: It mainly used to store the data.

                    How to create static buffer?

                              Go to: TBox Automation Tool > Buffer Operations >  TBox Set Buffer (Drag & Drop)

                                              Name                   Value
                                              BufferName             Anyvalue

            Syntax:  **{B[BufferName]} **
                  
                    
            2.Dynamic Buffer: It's used to capture the InnerText of the particular control and to stores it into the buffers.

            Syntax:  **{XB[BufferName]}**


     #8 **CARDINALITY**: It is a module attribute property and which allows us to add multiple attributes to the test step.

               Cardinality Default Value : 0-1
    


    #9 **Repetitions:** 

          Where do you find the Repetition property? 
               Repetition property exists in Test Step Folder


    #10 **Dynamic Expressions**: 

          {DATE} : it's used to pick the current date of the system

           Tosca's default date format:  dd.MM.yyyy


     Syntax:  {DATE[][][]}

           Examples:
                    {DAY} : Current date {30,24,12,20 etc….}
                    {ADAY} : Which day {Sat,Fri,mon,Tue etc….}
                    {LDAY}: Which day {Saturday,Monday,Tuesday….}
                    
                    {Month}:  example {9,10,11,12,2,3,4,etc….}
                    {Amonth}:  {Sep,Oct…..}
                    {Lmonth}: {September,October}
                    
                    {year}:   {23,22,21,20,19…..}
                    {Lyear}: {2023,2022,2021,2020 etc….}


       #11  TEST MANDATES: Test Mandates are used to avoid the overwrite of other test results.


       #12 **Data Driven Testing by using EXCEL Sheet**:

             - Go to "C" - drive 
             - Click on Tosca_Projects
             - Click on ToscaCommander
             - Click on Templates
             - Click on BO Folder
             - Copy Example excel  and paste it in any other folder
             - Open the copied file
             - Follow below format and enter the data 

Object/Attribute		omain	         TC_001	         TC_002	          TC_003

Gender					M 	         F	          M
First name				hello	         hello1	          hello2
Last name					pollo	         pollo1	          pollo2
Email					hp_abc@gmail.com   hp_def@gmail.com	hp_ghi@gmail.com
Password					1234567	         hp123456	          gh123456
Confirm password				1234567	         hp123456	          gh123456


              - Create one folder under TestCases Section
              - Add existing TestCase or New Test  cases
              - Right click and click on  "Convert to Template"
              
                       In Properties :
                                SchemaPath (Click on ..)
                                Data Source Path : <path of excel>
                                Worksheet: <sheetname> 
                                Click on Ok
                                SchemaName: <once uploaded it’ll update>
               - Remove hardcoded values and follow the below syntax to enter the column names in the Text fields
                      For example:
                                Gender : {XL[Gender}
                                First Nam: {XL[First Name]} etc.......

               - Right click  on the Template
               - Click on Ellipses … (three dots)
               - Select "Create TemplateInstance"
               - One pop up will display {to check the path and sheetname}
               - Another pop up YES or NO – click on YES
               - TemplateInstance Folder will created
               - Right click on TemplateInstance and click on run.


              
                       
 

               
