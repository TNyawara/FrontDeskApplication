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
        JLabel namelabel=new JLabel("Name: ");
        JTextField name=new JTextField();
        name.setColumns(25);
        JButton submit=new JButton("Submit");
        mypanel.add(namelabel);
        mypanel.add(name);
        mypanel.add(submit);
        myframe.add(mypanel);
        myframe.setSize(900,500);
        myframe.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        myframe.setVisible(true);
    }
    
}

