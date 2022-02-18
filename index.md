# Vilaysith Phongsavath - SNHU Capstone ePortfolio
## CS-499
------------------------------------------------------------

### This portfolio contains three programming projects, a video, and a self assessment
### Final - Self Assessment
### Milestone 1 - Code Review and Plans (Video)
### Milestone 2 - Software Design and Engineering (pet.java,jframe)
### Milestone 3 - Data Structures and Algorithms (petsView.java,jframe,mysql) 
### Milestone 4 - Databases (registration.java,jframe,jdbc,mysql)

-------------------------------------------------------------

## Self - Assessment:

### Overview:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;More than an achievement I have accomplished through the course and that shows up in multiple skills I gained and used them to enhance the code starting from the software design category where I focused on delivering quality work and sharing a clear code to build up a collaborative environment, moving to the data structure section where I used some new algorithms and applied new practices while managing the trade-offs involved earlier in the software design. 
Finally, in the databases category where I used a simple artifact and connected it to the existing code, in addition, I surfed the internet to get some workarounds to be able to use the available tool NetBeans and I was able to accomplish the task successfully.
I noticed that I have a better security mindset in all the project categories, especially while creating the access to the database administrator, however, I feel that this part should be improved in the future as I need to always keep in mind that passwords must be complex to avoid easy cracking, so the combination of uppercase, lowercase letters, numbers, and special characters is mandatory all-time in the code; either if I am the user who is creating the credentials or I am the developer who is developing the code. 
So, I will consider this part in the future and I will make sure to add a clear pop-up in such a case to educate the users on how to create complex passwords. This point shows up that I become more proactive and my productivity is improved over the course.

#### Team Environments:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;When it comes to collaborating in a team environment,Learning how to use Git helped me to better understand its various features. I think that it is the main source of collaboration and team environments. Having this knowledge is very important for any team member.

#### Communicating to Stakeholders:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I believe that my projects directly communicate with stakeholders. The program I develop allows the stake holders to be able to easily add or delete their pet also veiw all of the pets in the database.

## Milestone 1 - Code Review video
link to the code review https://www.youtube.com/watch?v=ko3zrZhegww&t=5s

## Milestone 2 - Software Design and Engineering
### Converting original command line txt java code into a more user friendly graphic user inteface with added security features in a form of a username and password

#### Artifact Description:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;My artifact for milestone two is based off of a project from my IT-145 course.I used the pets’ shop code I developed earlier in IT-145 (Foundation in Application Development). This artifact was created around October 2019, I have learned a lot of concepts since then so I used these qualities in enhancing the software design and code structure and link it with another search engine structure code I created later in CS-260 (Data Structures and Algorithms: Analysis and Design) in early 2021. 
Java Swing JFrame class is the main artifact I used in this part to enhance the graphical user interface as it is typically the foundation for creating graphical Java applications. So, I imported javax.swing package. Also, I used the JDialog package to control the top-level window while inserting the Pets’ data, it inherits the Dialog class and it is a part Java swing package, I used this class as it can be customized based on the business need. Basically, the JDialog constructor is used to initiate a modeless dialog without a specified Frame owner and without a title.

### Artifact Enhancement Process:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Quality work starts by keeping every single detail in the project documented, I added more comments in the code to clarify the purpose of adding each portion of the code, I ensured to declare all the variables and that helped me to avoid Undefined Errors. So, I see that I succeeded in keeping the software design clear and simple which is one of the main course outcomes.

### Artifact inclusion:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;By using javax.swing package, I enhanced the code design so both the administrators and users can navigate between tabs easily and the new design allows the users to enter the pets’ data easily which is a great skill I learned over the course; when it comes to delivering a professional design, we should deliver a quality work that gives the end-users oral, written, and visual communications and make them feel that the application design is friendly.

## Milestone 3 and 4 - Algorithms and Data Structures and Databases

#### Artifact Description:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I used the Binary Search Algorithm to perform the search on the pets’ dataset. It counts on continuously dividing the whole portion of the list into chunks that could contain the required item until it narrows down the results to one possible item by using the time complexity O(log2N). I imported the dataset java.sql, then, started applying this methodology to the code, after that, when you search for the name of a pit in a sorted list of pets, the algorithm performs the binary search to return the best match based on a string-matching on the stemmed keywords.

### Artifact Enhancement Process:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Currently, I know more about data structure techniques and how are they breaking data down into terms to easily store them in the database and call them quickly when running the queries which is called the indexing process, basically, this helps in minimizing the number of disk accesses while processing queries, in addition, in large databases, we do not need to hammer databases each time we call an item. The search terms are generated using an analyzer that stems each word to its root form, this process helps the system in suggesting results according to the stemmed keywords. 
This artifact helped me use one of the skills I gained over the course and that shows up in using new packages like java.sql and ensured to declare all the variables in the program, also, I loaded MySQL driver successfully to the registration code and developed a connection between the local JDBC MySQL driver and the portal that is developed by java initially 

### Artifact inclusion:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I created a portal to be able to search for pets and filter them easily, I used some other known algorithms such as BFS (Breadth-First Search) or DFS (Distributed File System) for data indexing and getting the results easier and faster from the database, this practice evolved my experience in both linear and binary searches and helped me practically in enhancing the current software code and creating the portal view in a practical way.
I added a new portal view in the code structure so when users click on the View Pets button, it shows up another window and lets the users be able to start searching in DB.I imported java.sql to get all classes from the package java.sql at once, then, completed the connection setup by declaring the DB location and credentials to allows the code issues SQL queries to the database, I noticed that the password is not complex at all which is something I will keep in mind in a production environment for security purposes as the security mindset is one of the helpful concepts I learned over the course. Other than this, I added an insert method to insert the pets’ values into DB and to show up the message Saved Successfully once the record is inserted properly. In addition, I added a quick catch that an error has occurred when you cannot find what you are looking for, this is one of the most interesting concepts I learned in this course, I should give the user a clear error message to help identify and troubleshoot the issues easier.

### Original pet.java code 

import java.util.Scanner;

public class Pet {

    // Instance private Variables
    private String petType;
    private String petName;
    private int petAge;
    private int dogSpace;
    private int catSpace;
    private int daysStay;
    private double amountDue;

    // Default constructor for Pet class
    public Pet(String petType, String petName, int petAge, int dogSpace, int catSpace, int daysStay, double amountDue) {
        this.petType = petType;
        this.petName = petName;
        this.petAge = petAge;
        this.dogSpace = dogSpace;
        this.catSpace = catSpace;
        this.daysStay = daysStay;
        this.amountDue = amountDue;
    }

    // checkIn method
    public void checkIn() {

        // initial Cat space
        setCatSpace(12);

        // intial Cat space
        setDogSpace(30);

        System.out.print("Welcome, are you checking in a dog or cat:");

        // input from Scanner class
        Scanner input = new Scanner(System.in);
        String userChoice = input.nextLine();

        // determine if user is checking in a cat or dog
        if (userChoice.equals("cat")) {
            System.out.println("meow meow");
            // check if cat space is available
            if (getCatSpace() >= 1) {
                System.out.println("Cat space availalbe hooray!");
                System.out.println("Is your Cat a 'new' or 'returning' visitor?");
                // check if user cat is a new or returning visitor
                String catVisitor = input.nextLine();
                if (catVisitor.equals("new")) {
                    System.out.println("Hey new visitor");
                    System.out.println("Please allow us to collect some information about your cat:");
                    System.out.println("What is your Cat name?");
                    String newCatName = input.nextLine();
                    setPetName(newCatName);
                    System.out.println("How old is your Cat?");
                    int newCatAge = input.nextInt();
                    setPetAge(newCatAge);
                    
                    System.out.println("How many days will your Cat be staying with us?");
                    int catDays = input.nextInt();
                    // set the amount of days 
                    setDaysStay(catDays);

                    System.out.println("Thank you for the cat information!");
                    // decrease the avaialble slot of cat space by one
                    int currentCatSpace = getCatSpace();
                    setCatSpace(currentCatSpace - 1);

                } else if (catVisitor.equals("returning")) {
                    System.out.println("It is good to see you again!");
                    System.out.println("Please let us update some of your cat information");

                    System.out.println("How many days will your Cata be staying with us?");
                    int catDays = input.nextInt();
                    // set the amount of days for returning cats
                    setDaysStay(catDays);

                    // decrease avaialble cat space
                    int currentCatSpace = getCatSpace();
                    setCatSpace(currentCatSpace - 1);
                    updatePet();

                }

            } else {
                System.out.println("Sorry no room left in Cat space");

            }
        } else if (userChoice.equals("dog")) {
            System.out.println("woof woof");
            // check if dog space is available
            if (getDogSpace() >= 1) {
                System.out.println("Dog space availale hooray!");
                System.out.println("Is your Dog a 'new' or 'returning' visitor?");
                // check is user Dog is a new or returning visitor
                String dogVisitor = input.nextLine();
                if (dogVisitor.equals("new")) {
                    System.out.println("Welcome new visitor!");
                    System.out.println("Please allow us to collect some information about your dog:");
                    System.out.println("What is your dog name?");
                    String newDogName = input.nextLine();
                    setPetName(newDogName);
                    System.out.println("Now how old is your dog?");
                    int newDogAge = input.nextInt();
                    setPetAge(newDogAge);

                    System.out.println("How many days will your dog be staying with us?");
                    int dogDays = input.nextInt();
                    // check if grooming services for dogs are needed
                    if (dogDays >= 2){
                        System.out.println("Grooming services are avaialble for your dog!");
                    } else{
                        System.out.println("Grooming is not availalbe for your dog");
                    }

                    System.out.println("Thank you for the dog information!");

                    // decrease dog space by 1
                    int currentDogSpace = getDogSpace();
                    setDogSpace(currentDogSpace - 1);
                } else if (dogVisitor.equals("returning")) {
                    System.out.println("It is good to see you again!");
                    System.out.println("Please allow us to update some of your dog information");

                    System.out.println("How many days will your dog be staying with us?");
                    int dogDays = input.nextInt();
                    // check if grooming for returning dogs is needed 
                    if(dogDays >= 2){
                        System.out.println("Grooming services are available for your dog!");
                    } else{
                        System.out.println("Grooming is not available for your dog");
                    }

                    // decrease dog space by 1 for returning
                    int currentDogSpace = getDogSpace();
                    setDogSpace(currentDogSpace - 1);
                    updatePet();
                }

            } else {
                System.out.println("Sorry no room left in Dog space");
            }
        } else{
            System.out.println("Invalid choice, please select 'cat or 'dog'");
            checkIn();
        }

        // checkIn();
    }

    // checkOut method
    public void checkOut() {

        checkOut();
    }

    // getPet method
    public void getPet() {
        getPet();
    }

    // createPet method
    public void createPet() {
        createPet();
    }

    // updatePet method
    public void updatePet() {
        //updatePet();
    }

    

    public String getPetType() {
        return petType;
    }

    public void setPetType(String petType) {
        this.petType = petType;
    }

    public String getPetName() {
        return petName;
    }

    public void setPetName(String petName) {
        this.petName = petName;
    }

    public int getPetAge() {
        return petAge;
    }

    public void setPetAge(int petAge) {
        this.petAge = petAge;
    }

    public int getDogSpace() {
        return dogSpace;
    }

    public void setDogSpace(int dogSpace) {
        this.dogSpace = dogSpace;
    }

    public int getCatSpace() {
        return catSpace;
    }

    public void setCatSpace(int catSpace) {
        this.catSpace = catSpace;
    }

    public int getDaysStay() {
        return daysStay;
    }

    public void setDaysStay(int daysStay) {
        this.daysStay = daysStay;
    }

    public double getAmountDue() {
        return amountDue;
    }

    public void setAmountDue(double amountDue) {
        this.amountDue = amountDue;
    }

}

### Enhanced Pet.java

package com.mycompany.petsnew;

import javax.swing.JDialog;
    import javax.swing.JOptionPane;
    import javax.swing.WindowConstants;

    /**
     *
     * @author Vilaysith Phongsavath
     */
    /**Declaration for the class javax.swing.JFrame */

    public class Pets extends javax.swing.JFrame {

        /**
         * Creates new form dashboard
         */
	/** It is used to share the data story*/    

    /** defined as per the requirement of the program to handle the operation in the */
	/** WindowClosing method of a registered object that is WindowListener */

        public Pets() {
            initComponents();
                    setDefaultCloseOperation(WindowConstants.DO_NOTHING_ON_CLOSE);
        }

        /**
         * This method is called from within the constructor to initialize the form.
         */
	/** Method is also declared private and can not be accessed by any other method.*/
        @SuppressWarnings("unchecked")
        
        private void initComponents() {
	
	/** Will display short string or image or text */

            jLabel1 = new javax.swing.JLabel();
            jLabel2 = new javax.swing.JLabel();
            jButton1 = new javax.swing.JButton();
            jButton2 = new javax.swing.JButton();
            btnLogout = new javax.swing.JButton();
            btnHelp = new javax.swing.JButton();
            jLabel3 = new javax.swing.JLabel();

            setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
            setPreferredSize(new java.awt.Dimension(1360, 700));
            setSize(new java.awt.Dimension(1360, 700));
            setType(java.awt.Window.Type.UTILITY);

            jLabel1.setFont(new java.awt.Font("Tahoma", 1, 36)); 
            jLabel1.setText("Pet Store");

            jLabel2.setFont(new java.awt.Font("Tahoma", 1, 18)); 
            jLabel2.setForeground(new java.awt.Color(0, 0, 204));
            jLabel2.setText("Pets Manager");

            jButton1.setBackground(new java.awt.Color(0, 0, 102));
            jButton1.setFont(new java.awt.Font("Tahoma", 1, 18)); 
            jButton1.setForeground(new java.awt.Color(255, 255, 255));
            jButton1.setText("Add New Pet");
            jButton1.addActionListener(new java.awt.event.ActionListener() {
                public void actionPerformed(java.awt.event.ActionEvent evt) {
                    jButton1ActionPerformed(evt);
                }
            });

            jButton2.setBackground(new java.awt.Color(0, 0, 102));
            jButton2.setFont(new java.awt.Font("Tahoma", 1, 18)); 
            jButton2.setForeground(new java.awt.Color(255, 255, 255));
            jButton2.setText("View Pets");
            jButton2.addActionListener(new java.awt.event.ActionListener() {
                public void actionPerformed(java.awt.event.ActionEvent evt) {
                    jButton2ActionPerformed(evt);
                }
            });

            btnLogout.setBackground(new java.awt.Color(0, 0, 102));
            btnLogout.setFont(new java.awt.Font("Tahoma", 1, 18)); 
            btnLogout.setForeground(new java.awt.Color(255, 255, 255));
            btnLogout.setText("Logout");
            btnLogout.addActionListener(new java.awt.event.ActionListener() {
                public void actionPerformed(java.awt.event.ActionEvent evt) {
                    btnLogoutActionPerformed(evt);
                }
            });

            btnHelp.setBackground(new java.awt.Color(0, 0, 102));
            btnHelp.setFont(new java.awt.Font("Tahoma", 1, 18)); 
            btnHelp.setForeground(new java.awt.Color(255, 255, 255));
            btnHelp.setText("Help?");
            btnHelp.addActionListener(new java.awt.event.ActionListener() {
                public void actionPerformed(java.awt.event.ActionEvent evt) {
                    btnHelpActionPerformed(evt);
                }
            });

            jLabel3.setFont(new java.awt.Font("Tahoma", 1, 12)); 
            jLabel3.setForeground(new java.awt.Color(0, 51, 153));
            jLabel3.setText("Welcome Admin!!! enjoy your session.");

	    /** GUI layout */
            javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
            getContentPane().setLayout(layout);
            layout.setHorizontalGroup(
                layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                .addGroup(layout.createSequentialGroup()
                    .addContainerGap()
                    .addComponent(jLabel3, javax.swing.GroupLayout.PREFERRED_SIZE, 245, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, 272, Short.MAX_VALUE)
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                        .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                            .addComponent(jLabel1)
                            .addGap(408, 408, 408))
                        .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                                .addComponent(jLabel2)
                                .addComponent(jButton2, javax.swing.GroupLayout.PREFERRED_SIZE, 251, javax.swing.GroupLayout.PREFERRED_SIZE)
                                .addComponent(jButton1, javax.swing.GroupLayout.PREFERRED_SIZE, 251, javax.swing.GroupLayout.PREFERRED_SIZE))
                            .addGap(492, 492, 492))
                        .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                            .addComponent(btnHelp, javax.swing.GroupLayout.PREFERRED_SIZE, 131, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addGap(546, 546, 546))
                        .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                            .addComponent(btnLogout)
                            .addGap(563, 563, 563))))
            );
            layout.setVerticalGroup(
                layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                .addGroup(layout.createSequentialGroup()
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                        .addComponent(jLabel1)
                        .addGroup(layout.createSequentialGroup()
                            .addContainerGap()
                            .addComponent(jLabel3, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)))
                    .addGap(18, 18, 18)
                    .addComponent(jLabel2)
                    .addGap(59, 59, 59)
                    .addComponent(jButton2)
                    .addGap(56, 56, 56)
                    .addComponent(jButton1)
                    .addGap(43, 43, 43)
                    .addComponent(btnHelp)
                    .addGap(45, 45, 45)
                    .addComponent(btnLogout)
                    .addContainerGap(83, Short.MAX_VALUE))
            );

            pack();
            setLocationRelativeTo(null);
        }

        private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) 
        new registration().setVisible(true);
          this.dispose();
    
        }

        private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {
           new  family().setVisible(true);
            this.dispose();
           
        }
      
        /** event_btnLogoutActionPerformed */
        private void btnLogoutActionPerformed(java.awt.event.ActionEvent evt) {
        int dialogResult = JOptionPane.showConfirmDialog(null, "Are you sure you want to log out?","Cofirm Logout!",JOptionPane.YES_NO_OPTION);
        if (dialogResult==JOptionPane.YES_OPTION){
              new login().setVisible(true);
            this.dispose();
            
        }else{
            JOptionPane.showMessageDialog(this, "Continue with your session!");
        }
            
        }
  
	/** FIRST:event_btnHelpActionPerformed */

        private void btnHelpActionPerformed(java.awt.event.ActionEvent evt) {
            JOptionPane.showMessageDialog(null, "Contact me on my cell (0123456789) or email(vilaysith.phongsavath@edu.snhu) for assistance or adjustments, thank you");
                // TODO add your handling code here:
        } /** event_btnHelpActionPerformed */

        /**
         * @param args the command line arguments
         */
        public static void main(String args[]) {
            /* Set the Nimbus look and feel */
            //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
            /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
            * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
            */
            try {
                for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                    if ("Nimbus".equals(info.getName())) {
                        javax.swing.UIManager.setLookAndFeel(info.getClassName());
                        break;
                    }
                }
            } catch (ClassNotFoundException ex) {
                java.util.logging.Logger.getLogger(Pets.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
            } catch (InstantiationException ex) {
                java.util.logging.Logger.getLogger(Pets.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
            } catch (IllegalAccessException ex) {
                java.util.logging.Logger.getLogger(Pets.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
            } catch (javax.swing.UnsupportedLookAndFeelException ex) {
                java.util.logging.Logger.getLogger(Pets.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
            }
            //</editor-fold>

            /* Create and display the form */
            java.awt.EventQueue.invokeLater(new Runnable() {
                public void run() {
                    new Pets().setVisible(true);
                }
            });
        }

        /** Variables declaration */
        private javax.swing.JButton btnHelp;
        private javax.swing.JButton btnLogout;
        private javax.swing.JButton jButton1;
        private javax.swing.JButton jButton2;
        private javax.swing.JLabel jLabel1;
        private javax.swing.JLabel jLabel2;
        private javax.swing.JLabel jLabel3;
        /** End of variables declaration */
    }

### petsView.java


package com.mycompany.petsnew;

/**
 *
 * @author Vilaysith Phongsavath
 */


/** Importing Java Swing to create UI elements */
import javax.swing.*;

/** Importing Java SQL library to connect and create database operations */

import java.sql.*;
import javax.swing.table.DefaultTableModel;

public class petsView extends javax.swing.JFrame {
    /**
     * Creates new form petsView
     */
    
    /** Initializing variables */

    private Connection connect = null;
    private Statement statement = null;
    private PreparedStatement preparedStatement = null;
    private ResultSet resultSet = null;
    
    public petsView() {
        
        initComponents(); /** Calling initComponents to create UI items */
        populateData(); /** Calling Populate data in constructor to populate the JSwing table as soon as an instance of petsView is created */
        setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE); /** Close (X) button will close the window once clicked.*/
    }
   
    
   
    @SuppressWarnings("unchecked")
    
    /** BEGIN:initComponents */

    private void initComponents() {

    /** Method is also declared private and can not be accessed by any other method.*/ 
         
	/** Initializing UI element items using swing library */

        jScrollPane2 = new javax.swing.JScrollPane();
        petsTable = new javax.swing.JTable();
        jButton1 = new javax.swing.JButton();
        jButton2 = new javax.swing.JButton();
        jTextField2 = new javax.swing.JTextField();
        jButton3 = new javax.swing.JButton();

        /** Creating UI table to populate database items */

        petsTable.setModel(new javax.swing.table.DefaultTableModel(
            new Object [][] {
                {null, null, null, null},
                {null, null, null, null},
                {null, null, null, null},
                {null, null, null, null}
            },
            new String [] {
                "ID", "Pet Name", "Pet Type", "Pet Age"
            }
        ) {
            boolean[] canEdit = new boolean [] {
                false, false, false, false
            };

            public boolean isCellEditable(int rowIndex, int columnIndex) {
                return canEdit [columnIndex];
            }
        });

        /** Add table to the window */

        jScrollPane2.setViewportView(petsTable);

        /** Modifying colors for buttons */

        jButton1.setBackground(new java.awt.Color(0, 0, 102));
        jButton1.setFont(new java.awt.Font("Tahoma", 1, 18)); 
        jButton1.setForeground(new java.awt.Color(255, 255, 255));
        jButton1.setText("Close");
        jButton1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton1ActionPerformed(evt);
            }
        });

        jButton2.setBackground(new java.awt.Color(0, 0, 102));
        jButton2.setFont(new java.awt.Font("Tahoma", 1, 18)); 
        jButton2.setForeground(new java.awt.Color(255, 255, 255));
        jButton2.setText("Search");
        jButton2.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton2ActionPerformed(evt);
            }
        });

        jButton3.setBackground(new java.awt.Color(0, 0, 102));
        jButton3.setForeground(new java.awt.Color(255, 255, 255));
        jButton3.setText("Reset Filter");
        jButton3.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton3ActionPerformed(evt);
            }
        });

        /** This is how swing sets up the layout using previously created GUI elements */

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addContainerGap()
                .addComponent(jScrollPane2, javax.swing.GroupLayout.PREFERRED_SIZE, 1100, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(layout.createSequentialGroup()
                        .addGap(32, 32, 32)
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                            .addComponent(jButton2, javax.swing.GroupLayout.DEFAULT_SIZE, 181, Short.MAX_VALUE)
                            .addComponent(jButton1, javax.swing.GroupLayout.DEFAULT_SIZE, 181, Short.MAX_VALUE)
                            .addComponent(jButton3, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)))
                    .addGroup(layout.createSequentialGroup()
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                        .addComponent(jTextField2, javax.swing.GroupLayout.PREFERRED_SIZE, 239, javax.swing.GroupLayout.PREFERRED_SIZE)))
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addComponent(jScrollPane2, javax.swing.GroupLayout.Alignment.TRAILING, javax.swing.GroupLayout.DEFAULT_SIZE, 700, Short.MAX_VALUE)
            .addGroup(layout.createSequentialGroup()
                .addContainerGap()
                .addComponent(jTextField2, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                .addComponent(jButton2, javax.swing.GroupLayout.PREFERRED_SIZE, 38, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addComponent(jButton3)
                .addGap(40, 40, 40)
                .addComponent(jButton1)
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE))
        );

        jButton3.getAccessibleContext().setAccessibleName("Reset Filter");

        pack();
    }

    /** END:initComponents */

    /** CLOSE BUTTON METHOD */

    /** FIRST:event_jButton1ActionPerformed */	

    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {
        this.dispose(); //Close current window

   /** Create a new instance of Pets which shows the main menu */

        new Pets().setVisible(true); 
    }

    /** LAST:event_jButton1ActionPerformed */

    /** SEARCH BUTTON METHOD */
    /** FIRST:event_jButton2ActionPerformed */
    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {
        
        try{
            /** This will load the MySQL driver, each DB has its own driver */
            Class.forName("com.mysql.jdbc.Driver");
            /** Setup the connection with the DB */
            connect = DriverManager
                    .getConnection("jdbc:mysql://localhost/pet_store?"
                            + "user=sqluser&password=password123");

            /** Statements allow to issue SQL queries to the database */
            statement = connect.createStatement();
            /** We're querying using the text field for search to create a simple database search.*/
            String query = "select * from pets where id ='" + jTextField2.getText() + "'";
            resultSet = statement
                    .executeQuery(query);
            /** Loop over the ResultSet, populating table with database information */
                while(resultSet.next()){
                   String id = String.valueOf(resultSet.getInt("id"));
                   String pet_name = resultSet.getString("petname");
                   String pet_type = resultSet.getString("pettype");
                   String pet_age = String.valueOf(resultSet.getInt("petage"));

                   String tbData[] = {id, pet_name, pet_type, pet_age};
                   DefaultTableModel tblModel = (DefaultTableModel)petsTable.getModel();
                   tblModel.setRowCount(0); //Make sure to start with 0 rows to avoid empty rows in the table
                   tblModel.addRow(tbData);
          
                }
            
       }catch (Exception e){
           e.printStackTrace();
       }
    }

    /** RESET FILTER BUTTON */
    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {
       populateData(); //This calls populateData(); which populates the table with all data in the database.
    }

    /** POPULATE DATA -- This function connects to the database in order to populate the tables with all the data from database */
  private void populateData(){
      DefaultTableModel tblModel = (DefaultTableModel)petsTable.getModel();
      tblModel.setRowCount(0);
       try{
            /** This will load the MySQL driver, each DB has its own driver */
            Class.forName("com.mysql.jdbc.Driver");
            /** Setup the connection with the DB */
            connect = DriverManager
                    .getConnection("jdbc:mysql://localhost/pet_store?"
                            + "user=sqluser&password=password123");

            /** Statements allow to issue SQL queries to the database */
            statement = connect.createStatement();
            /** Result set get the result of the SQL query */
            resultSet = statement
                    .executeQuery("select * from pets");
            /** Looping over the result set to populate table */
            while(resultSet.next()){
               String id = String.valueOf(resultSet.getInt("id"));
               String pet_name = resultSet.getString("petname");
               String pet_type = resultSet.getString("pettype");
               String pet_age = String.valueOf(resultSet.getInt("petage"));
               
               String tbData[] = {id, pet_name, pet_type, pet_age};
               tblModel.addRow(tbData);
            }
       }catch (Exception e){
           e.printStackTrace();
       }
  }
              
           
        
    /**
     * @param args the command line arguments
     */
    public static void main(String args[]) {
       
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(petsView.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(petsView.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(petsView.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(petsView.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new petsView().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify//GEN-BEGIN:variables
    private javax.swing.JButton jButton1;
    private javax.swing.JButton jButton2;
    private javax.swing.JButton jButton3;
    private javax.swing.JScrollPane jScrollPane2;
    private javax.swing.JTextField jTextField2;
    private javax.swing.JTable petsTable;
    // End of variables declaration//GEN-END:variables
}

### registration.java


package com.mycompany.petsnew;

/**
 *
 * @author Vilaysith Phongsavath
 */
import java.sql.*;
import javax.swing.*;
import javax.swing.table.DefaultTableModel;

/**Declaration for the class javax.swing.JFrame */

public class registration extends javax.swing.JFrame {
    private javax.swing.JLabel petNameLabel;
    private javax.swing.JLabel petAgeLabel;
    private javax.swing.JLabel petTypeLabel;
    private javax.swing.JButton sveButton;
    private javax.swing.JButton cncelButton;
    private javax.swing.JTextField petNameField;
    private javax.swing.JTextField petAgeField;
    private javax.swing.JTextField petTypeField;
    private Connection connect = null;
    private PreparedStatement preparedStatement = null;
    
/** Creates new form dashboard */    

        public registration() {
            initComponents();
                setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    
        }
        
        @SuppressWarnings("unchecked")
  /** Method is also declared private and can not be accessed by any other method.*/  

    private void initComponents() {

/** Initializing UI element items using swing library */

        petNameLabel = new javax.swing.JLabel();
        petAgeLabel = new javax.swing.JLabel();
        petTypeLabel = new javax.swing.JLabel();
        sveButton = new javax.swing.JButton();
        cncelButton = new javax.swing.JButton();
        petNameField = new javax.swing.JTextField(20);
        petAgeField = new javax.swing.JTextField(2);
        petTypeField = new javax.swing.JTextField(20);

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setPreferredSize(new java.awt.Dimension(300, 300));
        setSize(new java.awt.Dimension(300, 300));
        setType(java.awt.Window.Type.UTILITY);
        
        petNameLabel.setFont(new java.awt.Font("Tahoma", 1, 12)); 
        petNameLabel.setText("Pet Name:");
        petAgeLabel.setFont(new java.awt.Font("Tahoma", 1, 12)); 
        petAgeLabel.setText("Pet Age:");
        petTypeLabel.setFont(new java.awt.Font("Tahoma", 1, 12)); 
        petTypeLabel.setText("Pet Type:");
  
        sveButton.setBackground(new java.awt.Color(0, 0, 102));
        sveButton.setFont(new java.awt.Font("Tahoma", 1, 18)); 
        sveButton.setForeground(new java.awt.Color(255, 255, 255));
        sveButton.setText("Save");
        sveButton.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                sveButtonActionPerformed(evt);
            }
    });
        cncelButton.setBackground(new java.awt.Color(0, 0, 102));
        cncelButton.setFont(new java.awt.Font("Tahoma", 1, 18)); 
        cncelButton.setForeground(new java.awt.Color(255, 255, 255));
        cncelButton.setText("Cancel");
        cncelButton.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                cncelButtonActionPerformed(evt);
            }
    });
        
 /** This is how swing sets up the layout using previously created GUI elements */
        
        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        layout.setAutoCreateGaps( true );
        layout.setAutoCreateContainerGaps(true);
            getContentPane().setLayout(layout);
            layout.setHorizontalGroup(layout.createSequentialGroup()
                .addGroup(layout.createParallelGroup( GroupLayout.Alignment.LEADING )
                    .addComponent(petNameLabel)
                    .addComponent(petAgeLabel)
                    .addComponent(petTypeLabel)
                    .addComponent(sveButton)
                    .addComponent(cncelButton)
                     
                )
                    
                .addGroup(layout.createParallelGroup( GroupLayout.Alignment.LEADING )
                    .addComponent(petNameField)
                    .addComponent(petAgeField)
                    .addComponent(petTypeField)
                )
                    
                    
            );
             layout.setVerticalGroup( layout.createSequentialGroup()
            .addGroup( layout.createParallelGroup( GroupLayout.Alignment.BASELINE )
                .addComponent(petNameLabel)
                .addComponent(petNameField) )
                     
            .addGroup( layout.createParallelGroup( GroupLayout.Alignment.BASELINE )
                .addComponent( petAgeLabel )
                .addComponent( petAgeField ) )
                     
            .addGroup( layout.createParallelGroup( GroupLayout.Alignment.BASELINE )
                .addComponent( petTypeLabel )
                .addComponent( petTypeField ) )
            .addGroup( layout.createParallelGroup( GroupLayout.Alignment.BASELINE )
                .addComponent( sveButton ) 
            )
                     
             .addGroup( layout.createParallelGroup( GroupLayout.Alignment.BASELINE )
                .addComponent( cncelButton ))
                    
                   
            );

        
    }

    /** SAVE BUTTON -- Inserting data from text fields into database */
    private void sveButtonActionPerformed(java.awt.event.ActionEvent evt) {
        
        
        try{
            /** This will load the MySQL driver, each DB has its own driver */
            Class.forName("com.mysql.jdbc.Driver");
            /** Setup the connection with the DB */
            connect = DriverManager
                    .getConnection("jdbc:mysql://localhost/pet_store?"
                            + "user=sqluser&password=password123");

            /** Statements allow to issue SQL queries to the database */
            
            /** Result set get the result of the SQL query */
            String query = "insert into pets values(default,?,?,?)";
            preparedStatement = connect.prepareStatement(query);
            preparedStatement.setString(1, petNameField.getText());
            preparedStatement.setString(2, petTypeField.getText());
            preparedStatement.setString(3, petAgeField.getText());
            preparedStatement.execute();
            JOptionPane.showMessageDialog(this, "Saved Successfully.");
            this.dispose();
            
            
       }catch (Exception e){
           e.printStackTrace();
           JOptionPane.showMessageDialog(this, e + "Has occurred.");

       }
        
        
}
    
    private void cncelButtonActionPerformed(java.awt.event.ActionEvent evt) {
        this.dispose();
}
    
}


