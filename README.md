# FrontDeskApplication
A simple front desk application that intergrates database
//Log in and log out(Session Management)
package front.deskapplication;

import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JPanel;
import javax.swing.JTextField;

/**
 *
 * @author Tiffany
 */
public class FrontDeskApplication {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // creating a Jframe
        JFrame myframe=new JFrame("Front Desk Application");
        JPanel mypanel=new JPanel();
        JLabel namelabel=new JLabel("Username: ");
        JLabel usernamelabel=new JLabel("Password: ");
        JTextField Username=new JTextField();
        JTextField password=new JTextField();
        Username.setColumns(10);
        password.setColumns(10);
        JButton login=new JButton("Login");
        mypanel.add(namelabel);
        mypanel.add(Username);
        mypanel.add(usernamelabel);
        mypanel.add(password);
        mypanel.add(login);
        myframe.add(mypanel);
        myframe.setSize(500,500);
        myframe.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        myframe.setVisible(true);
    }
    
}



//Dashboard
package Frame;

import java.awt.Color;
import java.awt.Frame;
import java.awt.GraphicsEnvironment;
import javax.swing.JFrame;

/**
 *
 * @author Tiffany
 */
public class Dashboard extends javax.swing.JFrame {

   static boolean maximized = true;
   int xMouse;
   int yMouse;
    public Dashboard() {
        initComponents();
        
    }

    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        panelHeader = new javax.swing.JPanel();
        Exit = new javax.swing.JButton();
        Minimize = new javax.swing.JButton();
        Maximize = new javax.swing.JButton();
        jScrollPane1 = new javax.swing.JScrollPane();
        Member = new javax.swing.JTable();
        ScrollBar = new javax.swing.JScrollBar();
        AddUser = new javax.swing.JButton();
        Logout = new javax.swing.JButton();
        Piechart = new javax.swing.JButton();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setTitle("Home");
        setUndecorated(true);
        setPreferredSize(new java.awt.Dimension(900, 600));
        setSize(new java.awt.Dimension(900, 600));

        panelHeader.setBackground(new java.awt.Color(204, 204, 204));
        panelHeader.addMouseMotionListener(new java.awt.event.MouseMotionAdapter() {
            public void mouseDragged(java.awt.event.MouseEvent evt) {
                panelHeaderMouseDragged(evt);
            }
        });
        panelHeader.addMouseListener(new java.awt.event.MouseAdapter() {
            public void mousePressed(java.awt.event.MouseEvent evt) {
                panelHeaderMousePressed(evt);
            }
        });

        Exit.setFont(new java.awt.Font("Tahoma", 1, 11)); // NOI18N
        Exit.setForeground(new java.awt.Color(102, 102, 102));
        Exit.setText("X");
        Exit.setBorder(null);
        Exit.setOpaque(false);
        Exit.addMouseListener(new java.awt.event.MouseAdapter() {
            public void mouseClicked(java.awt.event.MouseEvent evt) {
                ExitMouseClicked(evt);
            }
            public void mouseEntered(java.awt.event.MouseEvent evt) {
                ExitMouseEntered(evt);
            }
            public void mouseExited(java.awt.event.MouseEvent evt) {
                ExitMouseExited(evt);
            }
        });

        Minimize.setFont(new java.awt.Font("Tahoma", 1, 11)); // NOI18N
        Minimize.setText("-");
        Minimize.setOpaque(false);
        Minimize.addMouseListener(new java.awt.event.MouseAdapter() {
            public void mouseClicked(java.awt.event.MouseEvent evt) {
                MinimizeMouseClicked(evt);
            }
            public void mouseEntered(java.awt.event.MouseEvent evt) {
                MinimizeMouseEntered(evt);
            }
            public void mouseExited(java.awt.event.MouseEvent evt) {
                MinimizeMouseExited(evt);
            }
        });

        Maximize.setText("[]");
        Maximize.setOpaque(false);
        Maximize.addMouseListener(new java.awt.event.MouseAdapter() {
            public void mouseClicked(java.awt.event.MouseEvent evt) {
                MaximizeMouseClicked(evt);
            }
            public void mouseEntered(java.awt.event.MouseEvent evt) {
                MaximizeMouseEntered(evt);
            }
            public void mouseExited(java.awt.event.MouseEvent evt) {
                MaximizeMouseExited(evt);
            }
        });

        javax.swing.GroupLayout panelHeaderLayout = new javax.swing.GroupLayout(panelHeader);
        panelHeader.setLayout(panelHeaderLayout);
        panelHeaderLayout.setHorizontalGroup(
            panelHeaderLayout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, panelHeaderLayout.createSequentialGroup()
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                .addComponent(Maximize)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addComponent(Minimize)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addComponent(Exit, javax.swing.GroupLayout.PREFERRED_SIZE, 41, javax.swing.GroupLayout.PREFERRED_SIZE))
        );
        panelHeaderLayout.setVerticalGroup(
            panelHeaderLayout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addComponent(Exit, javax.swing.GroupLayout.Alignment.TRAILING, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
            .addComponent(Minimize, javax.swing.GroupLayout.DEFAULT_SIZE, 34, Short.MAX_VALUE)
            .addComponent(Maximize, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
        );

        Member.setModel(new javax.swing.table.DefaultTableModel(
            new Object [][] {
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null},
                {null, null, null, null, null, null}
            },
            new String [] {
                "First Name", "Last Name", "Gender", "Age", "Date Of Birth", "Telephone No."
            }
        ));
        jScrollPane1.setViewportView(Member);

        AddUser.setText("Add User");
        AddUser.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                AddUserActionPerformed(evt);
            }
        });

        Logout.setText("Logout");

        Piechart.setText("Pie Chart");
        Piechart.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                PiechartActionPerformed(evt);
            }
        });

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addComponent(panelHeader, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
            .addGroup(layout.createSequentialGroup()
                .addGap(37, 37, 37)
                .addComponent(ScrollBar, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(layout.createSequentialGroup()
                        .addComponent(AddUser)
                        .addGap(55, 55, 55)
                        .addComponent(Logout)
                        .addGap(96, 96, 96)
                        .addComponent(Piechart))
                    .addComponent(jScrollPane1, javax.swing.GroupLayout.PREFERRED_SIZE, 774, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addContainerGap(66, Short.MAX_VALUE))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addComponent(panelHeader, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, 251, Short.MAX_VALUE)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                        .addComponent(jScrollPane1, javax.swing.GroupLayout.PREFERRED_SIZE, 237, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addGap(34, 34, 34))
                    .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                        .addComponent(ScrollBar, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addGap(177, 177, 177)))
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(AddUser)
                    .addComponent(Logout)
                    .addComponent(Piechart))
                .addGap(21, 21, 21))
        );

        setBounds(0, 0, 900, 600);
    }// </editor-fold>                        

    private void ExitMouseEntered(java.awt.event.MouseEvent evt) {                                  
        Exit.setBackground(new Color(232,17,35));
    }                                 

    private void MinimizeMouseEntered(java.awt.event.MouseEvent evt) {                                      
    Minimize.setBackground(new Color(229,229,229));
    }                                     

    private void ExitMouseExited(java.awt.event.MouseEvent evt) {                                 
       Exit.setBackground(new Color(255,255,255));
    }                                

    private void MinimizeMouseExited(java.awt.event.MouseEvent evt) {                                     
       Minimize.setBackground(new Color(255,255,255));
    }                                    

    private void MaximizeMouseEntered(java.awt.event.MouseEvent evt) {                                      
        Maximize.setBackground(new Color(229,229,229));
    }                                     

    private void MaximizeMouseExited(java.awt.event.MouseEvent evt) {                                     
     Maximize.setBackground(new Color(255,255,255));
    }                                    

    private void ExitMouseClicked(java.awt.event.MouseEvent evt) {                                  
       System.exit(0);
    }                                 

    private void MinimizeMouseClicked(java.awt.event.MouseEvent evt) {                                      
        this.setState(Frame.ICONIFIED);
        
    }                                     

    private void MaximizeMouseClicked(java.awt.event.MouseEvent evt) {                                      
        if(maximized){
            Dashboard.this.setExtendedState(JFrame.MAXIMIZED_BOTH);
            GraphicsEnvironment env = GraphicsEnvironment.getLocalGraphicsEnvironment();
            Dashboard.this.setMaximizedBounds(env.getMaximumWindowBounds());
            maximized =false;
        }
        else{
            setExtendedState(JFrame.NORMAL);
            maximized = true;
        }
    }                                     

    private void panelHeaderMousePressed(java.awt.event.MouseEvent evt) {                                         
        xMouse=evt.getX();
        yMouse=evt.getY();
    }                                        

    private void panelHeaderMouseDragged(java.awt.event.MouseEvent evt) {                                         
       if(maximized){
           int x =evt.getXOnScreen();
            int y =evt.getYOnScreen();
            this.setLocation(x - xMouse, y - yMouse);
       }
    }                                        

    private void AddUserActionPerformed(java.awt.event.ActionEvent evt) {                                        
        // TODO add your handling code here:
    }                                       

    private void PiechartActionPerformed(java.awt.event.ActionEvent evt) {                                         
   
    }                                        

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
            java.util.logging.Logger.getLogger(Dashboard.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(Dashboard.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(Dashboard.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(Dashboard.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new Dashboard().setVisible(true);
            }
        });
    }
    
    // Variables declaration - do not modify                     
    private javax.swing.JButton AddUser;
    private javax.swing.JButton Exit;
    private javax.swing.JButton Logout;
    private javax.swing.JButton Maximize;
    private javax.swing.JTable Member;
    private javax.swing.JButton Minimize;
    private javax.swing.JButton Piechart;
    private javax.swing.JScrollBar ScrollBar;
    private javax.swing.JScrollPane jScrollPane1;
    private javax.swing.JPanel panelHeader;
    // End of variables declaration                   

}

