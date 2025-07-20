<h1 style="text-align:center;color:red;font-familly:sans-serif;">Requirement : Driving License Management System</h1>
<p style="font-style:italic;">The tasks of the Driver Licensing Department vary from country to another, but in general, these departments include a set of common and basic tasks to organize and manage the process of granting driving licenses and ensuring the provision of safe drivers on the roads.
These are the requirements of the first system in a simplified form, a general list of some simplified requirements for the services that the system will provide:</p>

<ol>
   <strong style="font-weight:bold;">The main services provided</strong>:
   <li>
        The service of issuing the driving license for the first time. Application fee is 15.00 dollars.
   </li>
   <li>
        Retake test service. Application fee is 5.00 dollars.
   </li>
   <li>
        The service of renewing the driving licenses. Application fee is 7.00 dollars.
   </li>
   <li>
        Issue a replacement for a lost driving license. Application fee is 15.00 dollars.
   </li>
   <li>
        Issue a replacement for a damaged driving license. Application fee is 5.00 dollars.
   </li>
   <li>
        Release a detained license service. Application fee is 15.00 dollars.
   </li>
   <li>
        Issue an international driving license. Application fee is 51.00 dollars.
   </li>
</ol>

<ul>
    <p style="font-weight:bold">To benefit from the service, the applicant must submit an application for the requested service and pay its fees. Application information:<p>
    <li>
        Application number ID (primary key)
    </li>
    <li>
        Application date
    </li>
    <li>
        Applicant Person ID, used to search the Applicant person through a textbox before making application, if the person does not exist then the user should add the person to the system.
    </li>
    <li>
        The application type chosen from the list provided above.
    </li>
    <li>
        The application status (new, cancelled, completed).
    </li>
    <li>
        The application fees.
    </li>
    <li>
        If the type of application is issuing a driver license for the first time then the license class should be chosen and the system check if the applicant has already an uncompleted application from the same class or the applicant has already an active driving license from the same class.
    </li>
</ul> 

<h3 style="color:#161616;">Every application is linked to one person, and every person can have multiple application.</h3> 
<ul>
    <p style="font-weight:bold;">The applicant’s information must be kept in the system and must not be repeated in the system. The applicant’s information is:</p>
    <li>
        The driver national identity card number(CIN)
    </li>
    <li>
        First Name and Last Name
    </li>
    <li>
        Birth date
    </li>
    <li>
        Address
    </li>
    <li>
        Phone number
    </li>
    <li>
        Email
    </li>
    <li>
        Nationality
    </li>
    <li>
        Personal photo
    </li>
</ul>
<ol>
    <p style="font-weight:bold;">The details of provided services:</p>
    <li>
        First-time license issuance service:
        <ul>
            <li>
                The applicant could apply to a license class. The licenses classes details are :
                <ul style="list-style:square">
                    <li>
                        <strong>Class 1</strong>: small motorcycle license. The minimum allowed age to apply is 18 years old, and the class fee is 15.00 dollars added to the application fee, the default validity length of the license is 5 years.
                    </li>
                    <li>
                        <strong>Class 2</strong>: heavy motorcycle license. The minimum allowed age to apply is 21 years old, and the class fee is 30.00 dollars added to the application fee, the default validity length of the license is 5 years.
                    </li>
                    <li>
                        <strong>Class 3</strong>: ordinary driving license (car license), it allows to the driver to drive the light vehicles and personal cars. The minimum allowed age to apply is 18 years old, and the class fee is 20.00 dollars added to the application fee, the default validity length of the license is 10 years.
                    </li>
                    <li>
                        <strong>Class 4</strong>: commercial driving license (taxi/limousine). The minimum allowed age to apply is 21 years old, and the class fee is 200.00 dollars added to the application fee, the default validity length of the license is 10 years.
                    </li>
                    <li>
                        <strong>Class 5</strong>: Agricultural and work vehicles used in farming or construction, (tractors / tillage machinery). The minimum allowed age to apply is 21 years old, and the class fee is 50.00 dollars added to the application fee, the default validity length of the license is 10 years.
                    </li>
                    <li>
                        <strong>Class 6</strong>: Small and medium bus license. The minimum allowed age to apply is 21 years old, and the class fee is 250.00 dollars added to the application fee, the default validity length of the license is 10 years.
                    </li>
                    <li>
                        <strong>Class 7</strong>: Truck and heavy vehicle license. The minimum allowed age to apply is 21 years old, and the class fee is 300.00 dollars added to the application fee, the default validity length of the license is 10 years.
                    </li>
                </ul> 
            </li>
        </ul>
        <p style="font-weight:bold;">Conditions for applying for a license according to the required category:</p>
        <ul>
           <li>
                Permissible driving age: The age of the applicant for a driving license must match the required age according to the category submitted. The system must reject the application if it violates the condition.
           </li>
           <li>
                The applicant must not have previously held the same driving license category. The system must reject the application if it violates the condition.
           </li>
           <li>
                The applicant can obtain more than one license from more than one category, for example, a small vehicle-driving license and a bicycle-driving license.
           </li>
           <li>
                Personal documents: Provide valid personal identity documents, such as a passport or national ID card.
           </li>
           <li>
               The next tests must be passed in order:
               <ul style="list-style:square">
                   <li>
                        The vision test: An appointment is set for this test and fee Is paid. Medical tests are conducted to verify the applicant's driving health and visual abilities and record the result in the system. Information about the date of the examination and the result must be kept, whether it was successful or failed. Test fee is $10. If the test failed, the system does not allow for continuation and granting a license. The applicant must correct his vision with either glasses or surgery and set another appointment of type retake test.
                   </li>
                   <li>
                        The written test: An appointment is set for this test and fee is paid.
                        After passing successfully the vision test, the applicant can choose the preferred date for passing the written test. The applicant is required to answer questions related to traffic laws and driving safety. The exam is paper-based outside the system, and the result is recorded in the system whether it is successful or failed, with a score of 100. The fee for this test is $20. In case of failing, the applicant can apply for retake test and pays its fee.
                   </li>
                   <li>
                        The street test: An appointment is set for this test and fee is paid after passing successfully the previous test (the written test). The appointment date is set manually by the user. The applicant must pass a practical driving test that assesses his or her ability to control the vehicle and comply with traffic rules.
                   </li>
                   <li>
                        After passing all the Tests, a driving license is issued based on applied class. The license info are : 
                        <ul>
                            <li>
                                License ID
                            </li>
                            <li>
                                The driver personal photo
                            </li>
                            <li>
                                The driver national identity card number(CIN)
                            </li>
                            <li>
                                The full Name of driver
                            </li>
                            <li>
                                The birth date of driver
                            </li>
                            <li>
                                The driving license class
                            </li>
                            <li>
                                Issue date
                            </li>
                            <li>
                                Expiration date
                            </li>
                            <li>
                                Additional Notes
                            </li>
                            <li>
                                Issue reason (new one, replacement for lost, replacement for damaged, renew)
                            </li>
                        </ul>
                   </li>
               </ul>
           </li>
           <li>
	            The system provides the service of inquiring about the licenses that a person hold through his national number (CIN) or license number. 
           </li>
           <li>
                If any license is issued to any person, this person becomes an official driver in the system with a given number. It is added once in the system and all future licenses are linked to it.
           </li>
        </ul>
    </li>
    <li>
        <p style="font-weight:bold;">Retake test service:</p>
        <ul>
            <li>
                This service allows setting a new appointment and retake test according to the type of test (vision, written, street).
            </li>
            <li>
                The applicant should fail before he can retake the test.
            </li>
            <li>
                Service fee is 5.00 dollars added to the fee of test based on its type.
            </li>
            <li>
                The user sets the appointment date manually.
            </li>
            <li>
                Every retake service is saved with a number that is linked to the original test application.
            </li>
            <li>
                It is not possible to schedule more than appointment while there is still an active appointment (not taken).
            </li>
        </ul>
    </li>   
    <li>
        <p style="font-weight:bold;">Renew driving license service :</p>
        <ul>
            <li>
                This service let drivers renew their expired driving licenses.
            </li>
            <li>
                The service fee is 7.00 dollars.
            </li>
            <li>
                The driver must deliver his expired license before he can get the new one.
            </li>
        </ul>
    </li>
    <li>
        <p style="font-weight:bold;">Issue replacement for a lost driving license service :</p>
        <ul>
           <li>
                This service allows the issuance of a replacement for a lost driving license.
           </li>
           <li>
                Service fee is 10.00 dollars.
           </li>
           <li>
                The system deliver a new license and deactivate the lost license in the system.
           </li>
        </ul>
    </li>
    <li>
        <p style="font-weight:bold;">Issue replacement for a damaged driving license service :</p>
        <ul>
            <li>
                This service allows the issuance of a replacement for a damaged driving license.
            </li>
            <li>
                The driver must deliver the damaged license in order to issue a replacement.
            </li>
            <li>
                Service fee is 5.00 dollars.
            </li>
        </ul>
    </li>
    <li>
        <p style="font-weight:bold;">Release detained license :</p>
        <ul>
            <li>
                This service allows licenses to be released after paying the fine fees resulting from the detainment, handing over the license to its owner, and recording the date of releasing the detained license in the system.
            </li>
            <li>
                Application fee is 15.00 dollars.
            </li>
            <li>
                The system save the detained licenses. A detained license info are:
                <p>Detain ID, Detained License ID, Detain date, Fine fee, The user that detain the license, Is released (Boolean), Release date,The user that release the license, Release application ID.</p>               
            </li>
        </ul>
    </li>
    <li>
        <p style="font-weight:bold;">
            Issue an international driving license service : 
        </p>
        <ul>
            <li>
                This service allows the issuance of an international driving license for a specific duration.
            </li>
            <li>
                This service is only available to drivers with license of class 3 (car license). The license must not be expired or detained to apply for this service.
            </li>
            <li>
                Service fee is 51.00 dollars.
            </li>
            <li>
                System should not let the issuing of an international driving license if there already an active one. In addition, the system should keep all the previous issued licenses. 
            </li>
        </ul>
    </li>
</ol>
<ol>
   <p style="font-weight:bold;">System management:</p>
   <li>
       <p style="font-weight:bold;">User management in the system :</p>
       <ul>
           <li>
                Add user by linking him to person in the system.
           </li>
           <li>
                Display user info.
           </li>
           <li>
                Modify login information.
           </li>
           <li>
                Delete user.
           </li>
           <li>
                Deactivate a user account.
           </li>
           <li>
                the user information are : User ID, CIN, Full Name, birth date, address, phone number, email, nationality, personal photo, login, password.
           </li>
       </ul>
   </li>
   <li>
       <p style="font-weight:bold;">People management in the system :</p>
       <ul>
           <li>
	            Search for a person by his CIN or Person ID or other info.	
           </li>
           <li>
                Display person info.
           </li>
           <li>
                Add new person to the system.
           </li>
           <li>
                Edit person info.
           </li>
           <li>
                Delete person info.
           </li>
           <li>
                The CIN is unique in the system.
           </li>
           <li>
                Person info are : Person ID, CIN, First Name, Last Name, birth date, address, phone number, email, nationality, person photo.
           </li>
       </ul>
   </li>
   <li>
       <p style="font-weight:bold;">
            Application types management : 
       </p>
       <ul>
            <li>
                Searching for application by Person ID or CIN.
            </li>
            <li>
                Display the applications list.
            </li>
            <li>
                Display the applications information and its fees.
            </li>
            <li>
                Edit the information of an application.
            </li>
            <li>
                Filtering the applications by status.
            </li>
       </ul>
   </li>
   <li>
       <p style="font-weight:bold;">Tests list management: the system allows just modifying the test fees.</p>
   </li>
   <li>
       <p style="font-weight:bold;">License classes management: the system allows modifying just the minimum allowed age, the default validity length and the class fee.</p>
   </li>
   <li>
       <p style="font-weight:bold;">Detain a driving license: the system allows detaining licenses, and setting the fine fee and detainment date and reason.</p>
       <ul>
       </ul>
   </li>
</ol>
















