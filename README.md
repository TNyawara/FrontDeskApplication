# FrontDeskApp
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
        JButton submit=new JButton("Submit");
        mypanel.add(namelabel);
        mypanel.add(Username);
        mypanel.add(usernamelabel);
        mypanel.add(password);
        mypanel.add(submit);
        myframe.add(mypanel);
        myframe.setSize(900,500);
        myframe.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        myframe.setVisible(true);
    }
    
}

//Dashboard
