# hostel-management-system-gui

package friends;

import java.awt.*;
import java.awt.event.*;
import javax.swing.*;
import javax.swing.event.*;
import javax.swing.table.*;
import java.util.*;
import java.net.*;


public class Project2 extends JPanel implements ActionListener,EventListener{
	
	JFrame f1,f2,f3,f4;
	 JLabel l,l1,l2,l3,l4,l5,l6,l7,l8,l9,l10,k1,k2,k3,k4,k5,k6;
	 Label a0,a1,a2,a3,a4,a5,a6,a11,a22,a33,a44,a55,a66;
	 JTextField t1,t2,t3,t4,t5,t6,t7,m1,m2,m3,m4,m5,m6;
	 JPasswordField p1,p2;
	 JButton b1,b2,b3,b4,b5,b6;
	
	 JRadioButton rb1,rb2,rb3,rb4;
	 ButtonGroup bg1,bg2;
	 String s1,s2,s3,s4;
	String name,regno,reason,from,to,gender;
	String namen,regnon,dob,room,block,cl;
	
	JFrame pro1,pro2,pro3,pro4,pro5,pro6;
    JLabel q01,q02,q11,q21,q31,q41,q51,q61,q71,q12,q22,q32,q42,q52,q62,q72,label;
    JTextField w1,w2,w3,w4,w5,w6;
    JButton bt1,bt2,bt3,bt4,bt5,bt6,bt7,bt8;
	String str1,str2,str3,str4,str5,str6;
	
	JButton mb1,mb2,mb3,mb4;

//	ImageIcon img01 = new ImageIcon(getClass().getResource("C:/ssv/project/img01.jpg")).getImage();
//	ImageIcon img02 = new ImageIcon(getClass().getResource("C:/ssv/project/img02.jpg")).getImage();
//	JLabel img1 = new JLabel("Image and Text",img01,JLabel.CENTER);
//	JLabel img2 = new JLabel("Image and Text",img02,JLabel.CENTER);
	 public Project2 () {
		
		 f1=new JFrame("Hostel login");
		 f2=new JFrame("Create an account");
		f3=new JFrame("Warden page");
		f4=new JFrame("Student page");
		 //f1
		 l=new JLabel("Login with your account");
		 l.setFont(new Font("Timesnewroman",Font.BOLD,20));
		 l1=new JLabel("User Name    :");
		 l2=new JLabel("Password     :");
		 JPanel j4=new JPanel();
		 j4.setLayout(null);
		 //f1 done
		 //f2
			l3=new JLabel("Create an account");
		 l3.setFont(new Font("Timesnewroman",Font.BOLD,20));
		 l4=new JLabel("Name                     :");
		 l5=new JLabel("Date of birth    :");
		 l6=new JLabel("Class    :");
		 l7=new JLabel("New password        :");
		 l8=new JLabel("Regsistration num   :");
		 l9=new JLabel("Room no           :");
		 l10=new JLabel("Block             :");
		  
		  rb1=new JRadioButton("Male");
			rb2=new JRadioButton("Female"); 
			bg1=new ButtonGroup();
			bg1.add(rb1);
			bg1.add(rb2); 
			//f2 done
			//f3-Admin
			a0 = new Label("Leave Application");
			a0.setFont(new Font("Timesnewroman",Font.BOLD,20));
			a1 = new Label(null);
			a2 = new Label(null);
			a3 = new Label(null);
			a4 = new Label(null);
			a5 = new Label(null);
			a6 = new Label(null);
			a11 = new Label("Name    :");
			a22 = new Label("Reg num   :");
			a33 = new Label("Gender    :");
			a44 = new Label("Date from :");
			a55 = new Label("Date till :");
			a66 = new Label("Reason    :");
			
			 a0.setBounds(130,8,600,100);
		 a1.setBounds(190,75,100,30);
		 a2.setBounds(190,105,100,30);
		a3.setBounds(190,135,100,30);
		a4.setBounds(190,165,100,30);
		a5.setBounds(190,195,100,30);
		a6.setBounds(190,225,100,30);
		a11.setBounds(80,75,100,30);
		a22.setBounds(80,105,100,30);
	   a33.setBounds(80,135,100,30);
	   a44.setBounds(80,165,100,30);
	   a55.setBounds(80,195,100,30);
	   a66.setBounds(80,225,100,30);	
			j4.add(a0);
			j4.add(a1);
			j4.add(a2);
			j4.add(a3);
			j4.add(a4);
			j4.add(a5);
			j4.add(a6);
		
			j4.add(a11);
			j4.add(a22);
			j4.add(a33);
			j4.add(a44);
			j4.add(a55);
			j4.add(a66);
			//f3-done
			//f4-student
			k1=new JLabel("Apply leave");
		 k1.setFont(new Font("Timesnewroman",Font.BOLD,20));
		 k2=new JLabel("Name                     :");
		 k3=new JLabel("Reg No :");
		 k4=new JLabel("Date from     :");
		 k5=new JLabel("Date to        :");
		 k6=new JLabel("Reason  :");
		  
		  rb1=new JRadioButton("Male");
			rb2=new JRadioButton("Female"); 
			  rb3=new JRadioButton("Male");
			rb4=new JRadioButton("Female"); 
			bg1=new ButtonGroup();
			bg2=new ButtonGroup();
			bg1.add(rb1);
			bg1.add(rb2);
				bg2.add(rb3);
			bg2.add(rb4);
		//f4-done
			
		 //f1
		  t1=new JTextField(20);
		 l.setBounds(150,10,300,100);
		 
		  l1.setBounds(80,75,150,30);
		  l2.setBounds(80,115,150,30);
		  p1=new JPasswordField(20);
		  b1=new JButton("Submit");
		  b2=new JButton("Create");
		  JPanel j1=new JPanel();
		  JPanel j2=new JPanel();
		   JPanel j3=new JPanel();
		   
		  j1.setLayout(null);
		  j2.setLayout(null);
		  j3.setLayout(null);
		  
		  
		  t1.setBounds(200,80,200,25);
		  p1.setBounds(200,120,200,25);
		 
		  b1.setBounds(150,180,100,30);
		  b2.setBounds(300,180,100,30);
		 
		  j1.add(t1); j1.add(l);
		  j1.add(p1);
		  j1.add(b1);
		  j1.add(b2);
		  j1.add(l1);j1.add(l2);
		  //f1-done
		  
		  
		  //f2
		   p2=new JPasswordField(20);
		  
		 l3.setBounds(130,8,600,100);
		 l4.setBounds(83,75,150,30);
		  l5.setBounds(80,115,150,30);
		l6.setBounds(81,155,150,30);
		l8.setBounds(81,195,150,30);
		l7.setBounds(81,235,150,30);
		l9.setBounds(81,275,150,30);
		l10.setBounds(81,315,150,30);
		
		rb1.setBounds(200,355,100,25);
  rb2.setBounds(300,355,100,25);
  
			b3=new JButton("Create the account");
			b4=new JButton("Go to login page");
			b6=new JButton("Go to login page");
		t2=new JTextField(20);
		t3=new JTextField(20);
		t4=new JTextField(20);
		t5=new JTextField(20);
		t6=new JTextField(20);
		t7=new JTextField(20);
		
		 t2.setBounds(200,80,200,25);
		 t3.setBounds(200,120,200,25);
		 t4.setBounds(200,160,200,25);
		 t4.setBounds(200,160,200,25);
		 t5.setBounds(200,200,200,25);
		 t6.setBounds(200,280,200,25);
		 t7.setBounds(200,320,200,25);
		 p2.setBounds(200,240,200,25);
		  
		   rb3.setBounds(200,360,100,25);
			rb4.setBounds(300,360,100,25);
		  b3.setBounds(100,400,180,30);
		   b4.setBounds(300,400,180,30);
		   
		  j2.add(rb1);
			j2.add(l3);
			j2.add(rb2);
		  j2.add(l4);
		  j2.add(l5);
		  j2.add(l6);
		  j2.add(l7);		  j2.add(l8);
		j2.add(l9);
		j2.add(l10);
		  j2.add(t2);j2.add(t6);j2.add(t7);
		  j2.add(t3);
		  j2.add(t5);
		  j2.add(b3); j2.add(b4);
		  j2.add(t4);j2.add(p2);
		  //f2-done
		  
		  
		  //f3
		  		   m1=new JTextField(20);
		  
		 k1.setBounds(130,8,600,100);
		 k2.setBounds(83,75,150,30);
		 k3.setBounds(80,115,150,30);
		k4.setBounds(81,155,150,30);
		k5.setBounds(81,195,150,30);
		k6.setBounds(81,235,150,30);
		
		
		
  
			b5=new JButton("Apply Leave");
		m2=new JTextField(20);
		m3=new JTextField(20);
		m4=new JTextField(20);
		m5=new JTextField(20);
		m6=new JTextField(20);
		 m1.setBounds(200,80,200,25);
		 m2.setBounds(200,120,200,25);
		 m3.setBounds(200,160,200,25);
		// m4.setBounds(200,160,200,25);
		 m5.setBounds(200,200,200,25);
		 m6.setBounds(200,240,200,25);
		  
		   rb3.setBounds(200,280,100,25);
			rb4.setBounds(300,280,100,25);
		  b5.setBounds(100,320,180,30);
		 b6.setBounds(300,320,180,30);
		   
		  j3.add(rb3);
			j3.add(k1);
			j3.add(rb4);
		  j3.add(k2);
		  j3.add(k3);
		  j3.add(k4);
		  j3.add(k5);		  j3.add(k6);

		  j3.add(m1);
		  j3.add(m2);
		  j3.add(m3);
		  j3.add(b5);j3.add(b6);
		  j3.add(m4);j3.add(m5);
		  j3.add(m6);
		  //f3-done
		  
		  //creating frames
		  f1.add(j1,BorderLayout.CENTER);
		  f2.add(j2,BorderLayout.CENTER);
		  f3.add(j4,BorderLayout.CENTER);
		  f4.add(j3,BorderLayout.CENTER);
		  f1.add(j1);
		  f2.add(j2);
		  f3.add(j4);
		  f4.add(j3);
		  f1.setSize(640,480);
		  f2.setSize(640,480);
		  f3.setSize(640,480);
		  f4.setSize(640,480);
		  f1.setVisible(true);
		  f2.setVisible(false);
		  f3.setVisible(false);
		  f4.setVisible(false);
		f1.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		f2.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		f3.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		f4.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		
		b1.addActionListener(this);
		 b2.addActionListener(this);
		 b3.addActionListener(this);
		  b4.addActionListener(this);
		  b5.addActionListener(this);
		  b6.addActionListener(this);

		  //profiles
		  //img1.setIcon(new ImageIcon(img01));
		  //img2.setIcon(new ImageIcon(img02));

		  pro1=new JFrame("1860474 profile");
		  pro2=new JFrame("1860476 profile");
		  pro3=new JFrame("1860474 logged in");
		  pro4=new JFrame("1860476 logged in");
		 
		   q01=new JLabel("Your Profile details");
		   q01.setFont(new Font("Timesnewroman",Font.BOLD,20));
		   q02=new JLabel("Your Profile details");
		   q02.setFont(new Font("Timesnewroman",Font.BOLD,20));
		   q11=new JLabel("Name                 : Sakala Lakshmi Priya");
		   q21=new JLabel("Registration number  : 1860474");
		   q31=new JLabel("Date of birth        : 1/12/2000");
		   q41=new JLabel("Class                        : 3Btcs-c");
		   q51=new JLabel("Block                        : D-Block");
		   q61=new JLabel("Room num             : 420");
		   q71=new JLabel("Total amount of fines: Rs.420");
		   q12=new JLabel("Name                 : Sushmita Nagraj");
		   q22=new JLabel("Reg num              : 1860476");
		   q32=new JLabel("Date of birth           : 26/1/2001");
		   q42=new JLabel("Class                       : 3Btcs-c");
		   q52=new JLabel("Block                       : D");
		   q62=new JLabel("Room num                   : 421");
		   q72=new JLabel("Total amount of fines: Rs.0");
		   w1=new JTextField();
		   w2=new JTextField();
		   w3=new JTextField();
		   w4=new JTextField();
		   w5=new JTextField();
		   w6=new JTextField();
		   bt1=new JButton("Go to login page");
		   bt2=new JButton("Back to 1860474");
		   bt3=new JButton("Go to login page");
		   bt4=new JButton("Back to 1860476");
		   bt5=new JButton(); 
   
		   str1="1860474";
		   str2="12345678";
		   str3="1860476";
		   str4="65035499";
   
   
		  JPanel jp1=new JPanel();
		   jp1.setLayout(null);
		   JPanel jp2=new JPanel();
		   jp2.setLayout(null);
		   JPanel jp3=new JPanel();
		   jp3.setLayout(null);
		   JPanel jp4=new JPanel();
		   jp4.setLayout(null);
			
				q01.setBounds(130,8,600,100);
				q11.setBounds(80,75,300,30);
				q21.setBounds(80,95,300,30);
				q31.setBounds(80,115,300,30);
				q41.setBounds(80,135,300,30);
				q51.setBounds(80,155,300,30);
				q61.setBounds(80,175,300,30);
				q71.setBounds(80,195,300,30);
				bt1.setBounds(50,220,150,30);
				bt2.setBounds(250,220,150,30);

				q02.setBounds(130,8,600,100);          
				q12.setBounds(80,75,300,30);
				q22.setBounds(80,95,300,30);
				q32.setBounds(80,115,300,30);
				q42.setBounds(80,135,300,30);
				q52.setBounds(80,155,300,30);
				q62.setBounds(80,175,300,30);
				q72.setBounds(80,195,300,30);
				bt3.setBounds(50,220,150,30);
				bt4.setBounds(250,220,150,30);
   
			//	img1.setBounds(450,65,500,400);
			//	img2.setBounds(450,65,500,400);

			//img1.setIcon(new ImageIcon(img01));
			//	img2.setIcon(new ImageIcon(img02));

			//	pro1.getContentPane().add(img1);
			//	pro2.getContentPane().add(img2);
   
			   jp1.add(q01);jp1.add(q11);jp1.add(q21);jp1.add(q31);jp1.add(q41);jp1.add(q51);jp1.add(q61);jp1.add(q71);
			   jp1.add(bt1);jp1.add(bt2);
			 pro1.add(jp1,BorderLayout.CENTER);
			   pro1.add(jp1);
   
			   jp2.add(q02);jp2.add(q12);jp2.add(q22);jp2.add(q32);jp2.add(q42);jp2.add(q52);jp2.add(q62);jp2.add(q72);
			   jp2.add(bt4);jp2.add(bt3);
			   pro1.add(jp2,BorderLayout.CENTER);
			   pro2.add(jp2);
   
			   bt1.addActionListener(this);
			   bt2.addActionListener(this);
			   bt3.addActionListener(this);
			   bt4.addActionListener(this);
   
			

			 //pro3
			 

			 bt5=new JButton("Profile of 1860474");
			 bt6=new JButton("Leave for 1860474");

			 bt5.setBounds(50,150,300,30);
			 bt6.setBounds(50,180,300,30);

			 bt5.addActionListener(this);
			   bt6.addActionListener(this);

			   jp3.add(bt5);jp3.add(bt6);
			   pro3.add(jp3);
			   pro3.setSize(640,480);
			 pro3.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
			 pro3.setVisible(false);

			   pro1.setSize(640,480);
			   pro2.setSize(640,480);
			   pro1.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
			   pro2.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
				   
			   pro1.setVisible(false);
			   pro2.setVisible(false);
			   //pro4
			   

  
			   bt7=new JButton("Profile of 1860476");
			   bt8=new JButton("Leave for 1860476");
  
			   bt7.setBounds(50,150,300,30);
			   bt8.setBounds(50,180,3000,30);
  
			   bt7.addActionListener(this);
				 bt8.addActionListener(this);
				 jp4.add(bt7);jp4.add(bt8);

				 pro4.add(jp4);
				 pro4.setSize(640,480);
			   pro4.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
			   pro4.setVisible(false);
		
		s3="Warden";
		s4="hostel";
		 
	 }
	


	public void actionPerformed(ActionEvent e) {
		String a,b;
		int c=0;
		String arg = e.getActionCommand();
		
		if(arg.equals("Submit")){
			a=t1.getText();
			b=p1.getText();
			if((a.equals(s1)&&(b.equals(s2)))){
			JOptionPane.showMessageDialog(null, "Login Sucessfull");
			f2.setVisible(false);
			f1.setVisible(false);
			f3.setVisible(false);
			f4.setVisible(true);
			pro1.setVisible(false);
			pro2.setVisible(false);
			pro4.setVisible(false);
			
			}
			else if ((a.equals(s3)&&(b.equals(s4)))){
				JOptionPane.showMessageDialog(null, "Login Sucessfull");
			f2.setVisible(false);
			f1.setVisible(false);
			f3.setVisible(true);
			f4.setVisible(false);
			pro1.setVisible(false);
			pro2.setVisible(false);
			pro3.setVisible(false);
			pro4.setVisible(false);
			
			}
			else if ((a.equals(str1)&&(b.equals(str2)))){
				JOptionPane.showMessageDialog(null, "Login Sucessfull");
			f2.setVisible(false);
			f1.setVisible(false);
			f3.setVisible(false);
			f4.setVisible(false);
			pro1.setVisible(false);
			pro2.setVisible(false);
			pro3.setVisible(true);
			pro4.setVisible(false);
			
		
			}
			else if ((a.equals(str3)&&(b.equals(str4)))){
				JOptionPane.showMessageDialog(null, "Login Sucessfull");
			f2.setVisible(false);
			f1.setVisible(false);
			f3.setVisible(false);
			f4.setVisible(false);
			pro1.setVisible(false);
			pro2.setVisible(false);
			pro3.setVisible(false);
			pro4.setVisible(true);
			
			
			}
			else{
				JOptionPane.showMessageDialog(null, "Error Login Failed");
				
			}
		}
	else if((arg.equals("Profile of 1860474"))) {
			pro3.setVisible(false);
				pro1.setVisible(true);
				f2.setVisible(false);
			f1.setVisible(false);
			f3.setVisible(false);
			f4.setVisible(false);
			pro4.setVisible(false);
			pro2.setVisible(false);

		}
		else if((arg.equals("Back to 1860474"))) {
			pro3.setVisible(true);
				pro1.setVisible(false);
				f2.setVisible(false);
			f1.setVisible(false);
			f3.setVisible(false);
			f4.setVisible(false);
			pro4.setVisible(false);
			pro2.setVisible(false);

		}
		
		else if(arg.equals("Leave for 1860474")){
			pro3.setVisible(false);
			f4.setVisible(true);
			pro4.setVisible(false);
			f2.setVisible(false);
			f1.setVisible(false);
			
			f3.setVisible(false);
	}
else if((arg.equals("Profile of 1860476"))) {
		pro4.setVisible(false);
		pro3.setVisible(false);
			pro2.setVisible(true);
			f2.setVisible(false);
			f1.setVisible(false);
			f3.setVisible(false);
			f4.setVisible(false);

	}
	else if((arg.equals("Back to 1860476"))) {
		pro4.setVisible(true);
		pro3.setVisible(false);
			pro2.setVisible(false);
			f2.setVisible(false);
			f1.setVisible(false);
			f3.setVisible(false);
			f4.setVisible(false);

	}
	else if(arg.equals("Leave for 1860476")){
		pro4.setVisible(false);
		pro3.setVisible(false);
		f4.setVisible(true);
		f2.setVisible(false);
			f1.setVisible(false);
			pro1.setVisible(false);
			pro2.setVisible(false);
			f3.setVisible(false);
}
		
		else if(arg.equals("Create")){
			f2.setVisible(true);
			f1.setVisible(false);
			f3.setVisible(false);
			f4.setVisible(false);
			pro1.setVisible(false);
			pro3.setVisible(false);
			pro2.setVisible(false);
			pro4.setVisible(false);
			
		}
		else if(arg.equals("Create the account")){
			 s1=t5.getText();
			s2=p2.getText();
			namen=t1.getText();
			dob=t2.getText();
			regnon=t3.getText();
			room=t5.getText();
			block=t6.getText();
			cl=t7.getText();
			JOptionPane.showMessageDialog(null, "Your accouunt has been created sucessfully");
		}
		else if(arg.equals("Go to login page")){
			f2.setVisible(false);
			f1.setVisible(true);
			f3.setVisible(false);
			f4.setVisible(false);
			pro1.setVisible(false);
			pro2.setVisible(false);
			pro3.setVisible(false);
			pro4.setVisible(false);

		}
		else if(arg.equals("Apply Leave")){
			JOptionPane.showMessageDialog(null, "Leave Applied Successfully");
		name=m1.getText();
		regno=m2.getText();
		from=m3.getText();
		to=m5.getText();
		reason=m6.getText();
			a11.setText(name);
			a22.setText(regno);
			a33.setText(gender);
			a44.setText(from);
			a55.setText(to);
			a66.setText(reason);
		
		}
		else if((rb1.isSelected())||(rb3.isSelected())){
		
		gender="Male";
		}
			else if((rb2.isSelected())||(rb4.isSelected())){
				gender="Female";
			}
				
	}
	
	public static void main (String[] args) {
		Project2 b = new Project2();
	
	}

}
