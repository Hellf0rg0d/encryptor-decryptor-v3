import java.awt.Color;
import java.awt.EventQueue;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JOptionPane;
import javax.accessibility.AccessibleHyperlink;
import javax.swing.Icon;
import javax.swing.ImageIcon;
import java.awt.Font;
import java.awt.Image;
import java.awt.SystemTray;
import java.awt.Toolkit;
import java.awt.TrayIcon;
import java.awt.TrayIcon.MessageType;
import java.awt.datatransfer.StringSelection;
import javax.swing.JPasswordField;
import javax.swing.SwingConstants;
import javax.swing.event.HyperlinkEvent;
import javax.swing.JButton;
import javax.swing.JCheckBox;
import javax.swing.JDialog;
import java.awt.event.ActionListener;
import java.awt.event.KeyEvent;
import java.io.File;
import java.io.FileWriter;
import java.time.LocalDateTime;
import java.time.format.DateTimeFormatter;
import java.util.Random;
import java.util.Scanner;
import java.util.concurrent.ScheduledExecutorService;
import java.awt.event.ActionEvent;
import javax.swing.JTextField;

public class Main {

	private JFrame frame;
	private JPasswordField raw;
	private JTextField d;
	private int c ,shift,kj = 0,qo,qq;
	private String last;
	private boolean show,morce,eww,valid;
	private int[] copypaste = new int[1000];
	

	/**
	 * Launch the application.
	 */
	
	public static String conv(char j) {
		  String [] morse = new String[200];
		morse [97] = ".-";
		morse [98] = "-...";
		morse[99] = "-.-.";
		morse [100] = "-..";
		morse [101] = ".";
		morse [102] = "..-.";
		morse [103] = "--.";
		morse [104] = "....";
		morse [105] = "..";
		morse [106] = ".---";
		morse [107] = "-.-";
		morse [108] = ".-..";
		morse [109] = "--";
		morse [110] = "-.";
		morse [111] = "---";
		morse [112] = ".--.";
		morse [113] = "--.-";
		morse [114] = ".-.";
		morse [115] = "...";
		morse [116] = "-";
		morse [117]= "..-";
		morse [118] = "...-";
		morse [119] = ".--";
		morse [120] = "-..-";
		morse [121] = "-.--";
		morse [122] = "--..";
int qq = j;
if(qq>96 && qq <123) {
	return morse[qq];
}
else {
	return null;
}

	}
	public static int ran() {
		Random rand = new Random();
		int k;
		k = rand.nextInt(9999999);
		for(int a = 0; a== 1;) {
			if(k<=10000000 && k>100000000) {
				a++;
				return k;
			}
		
			
		}
		return k;
	}
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					Main window = new Main();
					window.frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the application.
	 */
	public Main() {
		initialize();
	}

	/**
	 * Initialize the contents of the frame.
	 */
	private void initialize() {
		
		boolean isOn = Toolkit.getDefaultToolkit().getLockingKeyState(KeyEvent.VK_CAPS_LOCK);
		Color aColor = Color.decode("#246EE9");
		frame = new JFrame();
		frame.setResizable(false);
		frame.setBounds(100, 100, 800,600);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frame.getContentPane().setLayout(null);
		frame.getContentPane().setBackground(aColor);
		

		
		JButton alert = new JButton("");
		alert.setIcon(new ImageIcon(Main.class.getResource("/icon/icons8-info-60 (1).png")));
		alert.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				JOptionPane.showMessageDialog(frame,
					    "Caps is turned on turn in off pls And restart the Application :)",
					    "Warning",
					    JOptionPane.WARNING_MESSAGE);
			}
		});
		JLabel infoo3 = new JLabel("The Generated seed is ");
		infoo3.setFont(new Font("Arial", Font.BOLD, 20));
		infoo3.setForeground(Color.WHITE);
		infoo3.setBounds(10, 125, 242, 30);
	   infoo3.setVisible(false);
		//frame.getContentPane().add(infoo3);
		alert.setToolTipText("It Shows messages");
		alert.setBounds(726, 164, 50, 50);
		alert.setOpaque(false);
		alert.setContentAreaFilled(false);
		alert.setBorderPainted(false);
		alert.setFocusable(false);
		frame.getContentPane().add(alert);
		try {
			  Image image = Toolkit.getDefaultToolkit().createImage("icon.png");
		
		SystemTray tray = SystemTray.getSystemTray();
		TrayIcon trayIcon = new TrayIcon(image, "Capslock error");
		 trayIcon.displayMessage("Hello, World", "notification demo", MessageType.INFO);
		 trayIcon.setImageAutoSize(true);
	        //Set tooltip text for the tray icon
	        trayIcon.setToolTip("System tray icon demo");
		 tray.add(trayIcon);
		alert.setEnabled(true);
		alert.setVisible(true);
		}
		catch(Exception ex) {
			ex.printStackTrace();
		}
		
		if(isOn == true) {
			alert.setEnabled(true);
			alert.setVisible(true);
		}
		else {
			alert.setVisible(false);
			alert.setEnabled(false);
		}
		

		d = new JTextField();
		d.setFont(new Font("Arial", Font.BOLD, 15));
		d.setBounds(259, 65, 151, 20);
JLabel numerrss = new JLabel("Number of characters to shift");
		numerrss.setFont(new Font("Arial", Font.BOLD, 20));
		numerrss.setForeground(Color.WHITE);
		numerrss.setBounds(249, 11, 295, 55);
        d.setColumns(10);
		JLabel infoo2 = new JLabel("Max is 10");
		infoo2.setFont(new Font("Arial", Font.BOLD, 17));
		infoo2.setForeground(Color.WHITE);
		infoo2.setBounds(420, 64, 86, 20);
		frame.getContentPane().add(numerrss);
		frame.getContentPane().add(infoo2);
		frame.getContentPane().add(d);
		
		JButton setting = new JButton("");
		setting.setToolTipText("Settings of the Application");
		setting.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				JFrame frames = new JFrame();
				frames.setVisible(true);
				frames.setTitle("Settings v3");
				frames.setBounds(0, 0, 500, 350);
				frames.getContentPane();
				frames.getContentPane().setBackground(Color.WHITE);
				frames.getContentPane().setLayout(null);
				JCheckBox jcb = new JCheckBox();
				jcb.setToolTipText("If unchecked the Encrypted/Decrypted key will be copied to your clipboard and will not be visible! \n if Checked the output is visible and can be copied! ");
				JCheckBox jcb2 = new JCheckBox();
				jcb2.setToolTipText("If checked the Encrypted word/s are going to get encrypted again into Morse code \n if unchecked the Encrypted word/s will remain as it is \n to make the output visible make sure you have checked the Above Option!");
				JCheckBox jcb3 = new JCheckBox();
				jcb3.setToolTipText("Instead of Shifted the Characters the Application Randomly generates the seed and Encrypts it ");
				JCheckBox jcb4 = new JCheckBox();
				jcb4.setToolTipText("If Checked your key is limited for 24 hours else it valid till end!");
				if(morce == true ) {
					jcb2.setSelected(true);
				}
				else {
					jcb2.setSelected(false);
				}
				if(show == true) {
					jcb.setSelected(true);
				}
				else {
					jcb.setSelected(false);
				}
				if(eww == true) {
					jcb3.setSelected(true);
				}
				else {
					jcb3.setSelected(false);
				}
				if(valid == true) {
					jcb4.setSelected(true);
				}
				else {
					jcb4.setSelected(false);
				}
				
				jcb.setFocusable(false);
				jcb2.setFocusable(false);
				jcb3.setFocusable(false);
				jcb.setText(" Show Decrypted/Encrypted word? ");
				jcb.setBounds(2, 50, 422, 23);
				jcb.setBackground(Color.WHITE);jcb.setForeground(Color.black);
				jcb.setFont(new Font("Arial", Font.BOLD, 20));
				jcb.addActionListener(new ActionListener() {
					public void actionPerformed(ActionEvent e) {
						if(jcb.isSelected()) {
						show = true;
					}
						else {
							show = false;
						}
					}
				});
				frames.getContentPane().add(jcb);
				
				JLabel jl2 = new JLabel("Appearance");
				jl2.setEnabled(true);
				jl2.setBounds(0, 10, 500, 27);
				jl2.setFont(new Font("Arial", Font.PLAIN, 20));
				jl2.setForeground(Color.black);jl2.setBackground(Color.black);jl2.setHorizontalAlignment(SwingConstants.CENTER);
				frames.getContentPane().add(jl2);
				
				JLabel jl = new JLabel();
				jl.setEnabled(true);
				jl.setText("");
				jl.setIcon(new ImageIcon(Main.class.getResource("/icon/nega.png")));
				jl.setBounds(2, 35, 500, 1);
				frames.getContentPane().add(jl);
				
				JLabel jl3 = new JLabel();
				jl3.setEnabled(true);
				jl3.setText("");
				jl3.setIcon(new ImageIcon(Main.class.getResource("/icon/nega.png")));
				jl3.setBounds(2, 125, 500, 1);
				frames.getContentPane().add(jl3);
				
				JLabel jl4 = new JLabel("Accessibility");
				jl4.setEnabled(true);
				jl4.setBounds(0, 100, 500, 27);
				jl4.setFont(new Font("Arial", Font.PLAIN, 20));
				jl4.setForeground(Color.black);jl4.setBackground(Color.black);jl4.setHorizontalAlignment(SwingConstants.CENTER);
				frames.getContentPane().add(jl4);
				
				
				jcb2.setText(" Morse Code ");
				jcb2.setBounds(6, 135, 422, 23);
				jcb2.setBackground(Color.WHITE);
				jcb2.setFont(new Font("Arial", Font.BOLD, 20));
				jcb2.addActionListener(new ActionListener() {
					public void actionPerformed(ActionEvent e) {
						if(jcb2.isSelected()) {
						morce = true;
					}
						else {
							morce = false;
						}
					}
				});
				frames.getContentPane().add(jcb2);
				jcb3.setText(" Generate Random seeds? ");
				jcb3.setBounds(6, 175, 300, 23);
				jcb3.setFont(new Font("Arial", Font.BOLD, 20));
				jcb3.setBackground(Color.WHITE);
				jcb3.addActionListener(new ActionListener() {
					public void actionPerformed(ActionEvent e) {
						if(jcb3.isSelected()) {
						eww= true;
				
						infoo2.setVisible(false);
						infoo3.setVisible(true);
						frame.getContentPane().add(infoo3);

					numerrss.setText("Type the seed for decryption!");
						frame.getContentPane().add(d);
						frame.getContentPane().add(infoo2);
						frame.getContentPane().add(numerrss);
					}
						else {
							infoo3.setVisible(false);
							frame.getContentPane().add(infoo3);
							d.setVisible(true);
							infoo2.setVisible(true);
							numerrss.setText("Type the number to shift");
							numerrss.setVisible(true);
							frame.getContentPane().add(d);
							frame.getContentPane().add(infoo2);
							frame.getContentPane().add(numerrss);
							eww = false;
							
						//	JOptionPane.showMessageDialog(null, "Suck it!!");
						}
					}
				});
				frames.getContentPane().add(jcb3);
				jcb4.setText("Make the key valid only for 24-hours?");
				jcb4.setToolTipText("This Option makes your Encryptio/Decryption key valid only till next day");
				jcb4.setBackground(Color.WHITE);
				jcb4.setBounds(6, 210, 450, 25);
				jcb4.setFont(new Font("Arial", Font.BOLD, 20));
				jcb4.setFocusable(false);
				jcb4.addActionListener(new ActionListener() {
					public void actionPerformed(ActionEvent e) {
						if(jcb4.isSelected()) {
							valid = true;
						}
						else {
							valid = false;
						}
					}
				});
				frames.getContentPane().add(jcb4);
				
			}
		});
		setting.setIcon(new ImageIcon(Main.class.getResource("/icon/icons8-gear-50.png")));
		setting.setBounds(726, 91, 50, 50);
		setting.setOpaque(false);
		setting.setContentAreaFilled(false);
		setting.setBorderPainted(false);
		setting.setFocusable(false);
		frame.getContentPane().add(setting);
		
	
		JLabel seede = new JLabel("");
		seede.setForeground(Color.WHITE);
		seede.setFont(new Font("Arial", Font.BOLD, 20));
		seede.setBounds(20, 154, 254, 60);
		frame.getContentPane().add(seede);
			
				JLabel lblNewLabel_1 = new JLabel("Type the raw text");
		lblNewLabel_1.setHorizontalAlignment(SwingConstants.CENTER);
		lblNewLabel_1.setForeground(Color.WHITE);
		lblNewLabel_1.setFont(new Font("Arial", Font.BOLD, 30));
		lblNewLabel_1.setBounds(10, 179, 784, 79);
		frame.getContentPane().add(lblNewLabel_1);
		frame.setBackground(new Color(255, 255, 0));
		
		raw = new JPasswordField();
		raw.setFont(new Font("Arial", Font.BOLD, 30));
		raw.setBounds(272, 251, 272, 36);
		frame.getContentPane().add(raw);

		
		JButton cpy1 = new JButton("");
		
		cpy1.setIcon(new ImageIcon(Main.class.getResource("/icon/icons8-paste-60 (1).png")));
		cpy1.setBounds(367, 395, 60, 60);
		cpy1.setFocusable(false);
		cpy1.setOpaque(false);
		cpy1.setBorderPainted(false);
		cpy1.setContentAreaFilled(false);
		cpy1.setVisible(false);
		frame.getContentPane().add(cpy1);
		
		JButton cpy2 = new JButton("");
		cpy2.setIcon(new ImageIcon(Main.class.getResource("/icon/icons8-paste-60 (1).png")));
		cpy2.setOpaque(false);
		cpy2.setBorderPainted(false);
		cpy2.setContentAreaFilled(false);
		cpy2.setFocusable(false);
		cpy2.setVisible(false);
		cpy2.setBounds(30, 213, 60, 60);
		frame.getContentPane().add(cpy2);
		
		JLabel ans = new JLabel("");
		ans.setHorizontalAlignment(SwingConstants.CENTER);
		ans.setFont(new Font("Arial", Font.BOLD, 25));
		ans.setForeground(Color.WHITE);
		JButton en = new JButton("Encrypt");

		en.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				
				if(valid == true) {
					qo = ran();
					qq = qo;
					copypaste[0] = qq;
					cpy2.setVisible(true);
					cpy2.addActionListener(new ActionListener() {
						public void actionPerformed(ActionEvent e) {
							Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(Integer.toHexString(copypaste[0])),null);
						}
					});
					frame.getContentPane().add(cpy2);
					int [] jfk = new int[8];
					 int b = 0;
					   while (qo > 0) {
					     
					       jfk[b] = qo%10;
					       qo = qo / 10;
					       b++;
					   }
					
					try {
						DateTimeFormatter dtf = DateTimeFormatter.ofPattern("dd"); 
						 LocalDateTime now = LocalDateTime.now();  
						  int twofour= Integer.parseInt(dtf.format(now));
					      twofour = twofour%10;
						seede.setText(Integer.toHexString(qq));
						String loc = System.getProperty("user.home");
						File file = new File(loc+"\\sc.txt");
						FileWriter wri = new FileWriter(file,true);

					char a[] = raw.getText().toCharArray();
					int c ,shift;
					
					shift = jfk[twofour];
					for(int size = 0;size<a.length;size++) {
						
						
						c = a[size];
					if(c<=96 || c >= 123) {
						wri.write((char)c);
					}
						
						if(a[size] > 96 &&a[size] < 123) {
							c = c+shift;
							if(c>122) {
								c =a[size]-26+shift;
								
							}
							else {
								
							}
							wri.write((char)c);
						}
						else {
						}					  
					}
					wri.close();
					Scanner sc = new Scanner(file);
					last = sc.nextLine();
					sc.close();		
					file.delete();
					if(show == true) {
						cpy1.setVisible(true);	
						ans.setText(last);
						cpy1.addActionListener(new ActionListener() {
							public void actionPerformed(ActionEvent e) {
								Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
							}
						});
						frame.getContentPane().add(cpy1);
						}
					else {
						Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
					}
					}
					
					catch (Exception ex) {
						ex.printStackTrace();
						
					}
					
				}
				else {
	
				if(eww == true) {
					qo = ran();
					qq = qo;
					copypaste[0] = qq;
					cpy2.setVisible(true);
					cpy2.addActionListener(new ActionListener() {
						public void actionPerformed(ActionEvent e) {
							Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(Integer.toHexString(copypaste[0])),null);
						}
					});
					frame.getContentPane().add(cpy2);
					int [] jfk = new int[8];
					 int b = 0;
					   while (qo > 0) {
					     
					       jfk[b] = qo%10;
					       qo = qo / 10;
					       b++;
					   }
					
					try {
						seede.setText(Integer.toHexString(qq));
						String loc = System.getProperty("user.home");
						File file = new File(loc+"\\sc.txt");
						FileWriter wri = new FileWriter(file,true);

					char a[] = raw.getText().toCharArray();
					int c ,shift;
					
					shift = jfk[3];
					for(int size = 0;size<a.length;size++) {
						
						
						c = a[size];
					if(c<=96 || c >= 123) {
						wri.write((char)c);
					}
						
						if(a[size] > 96 &&a[size] < 123) {
							c = c+shift;
							if(c>122) {
								c =a[size]-26+shift;
								
							}
							else {
								
							}
							wri.write((char)c);
						}
						else {
						}					  
					}
					wri.close();
					Scanner sc = new Scanner(file);
					last = sc.nextLine();
			
					//System.out.println(last);
					sc.close();		
					file.delete();
					if(show == true) {
						cpy1.setVisible(true);	
						ans.setText(last);
						cpy1.addActionListener(new ActionListener() {
							public void actionPerformed(ActionEvent e) {
								Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
							}
						});
						frame.getContentPane().add(cpy1);
						}
					else {
						Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
					}
					}
					
					catch (Exception ex) {
						ex.printStackTrace();
						
					}
		
				}
				
				else {
					
				
				if(morce == true ) {
					try {
						String loc = System.getProperty("user.home");
						File file = new File(loc+"\\sc.txt");
						FileWriter wri = new FileWriter(file,true);
		
					char a[] = raw.getText().toCharArray();
					int c ,shift;
				
					shift = Integer.parseInt(d.getText());
					for(int size = 0;size<a.length;size++) {
						c = a[size];
					
						if(a[size] > 96 &&a[size] < 123) {
							c = c+shift;
							if(c>122) {
								c =a[size]-26+shift;
						
							}
							else {
							
							}
							wri.write(" ");
							wri.write(conv((char)c));
						}
						else {
						}					  
					}
					wri.close();
					Scanner sc = new Scanner(file);
					last = sc.nextLine();
			
				
					sc.close();		
					if(show == true) {
						cpy1.setVisible(true);	
						ans.setText(last);
						cpy1.addActionListener(new ActionListener() {
							public void actionPerformed(ActionEvent e) {
								Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
							}
						});
						frame.getContentPane().add(cpy1);
						}
					else {
						Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
					}
					}
					
					catch (Exception ex) {
						ex.printStackTrace();
						
					}
				}
				else {
				try {
					String loc = System.getProperty("user.home");
					File file = new File(loc+"\\sc.txt");
					FileWriter wri = new FileWriter(file,true);
	
				char a[] = raw.getText().toCharArray();
				int c ,shift;

				shift = Integer.parseInt(d.getText());
				for(int size = 0;size<a.length;size++) {
				
					
					c = a[size];
				if(c<=96 || c >= 123) {
					wri.write((char)c);
				}
					
					if(a[size] > 96 &&a[size] < 123) {
						c = c+shift;
						if(c>122) {
							c =a[size]-26+shift;
							
						}
						else {
							
						}
						wri.write((char)c);
					}
					else {
					}					  
				}
				wri.close();
				Scanner sc = new Scanner(file);
				last = sc.nextLine();
				sc.close();		
				file.delete();
				if(show == true) {
					cpy1.setVisible(true);	
					ans.setText(last);
					cpy1.addActionListener(new ActionListener() {
						public void actionPerformed(ActionEvent e) {
							Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
						}
					});
					frame.getContentPane().add(cpy1);
					}
				else {
					Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
				}
				}
				
				catch (Exception ex) {
					ex.printStackTrace();
					
				}
			}
			}
			}
			}
		});
		
		en.setForeground(Color.WHITE);
		en.setFont(new Font("Arial", Font.BOLD, 25));
		en.setOpaque(true);
		en.setFocusable(false);
		en.setContentAreaFilled(false);
		en.setBorderPainted(false);
		en.setBounds(259, 298, 143, 36);
		
		ans.setBounds(0, 352, 794, 30);
		frame.getContentPane().add(ans);
		frame.getContentPane().add(en);
		
		
		
		JButton info = new JButton("");
		info.setToolTipText("Shows the info/about the Application");

		info.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				JOptionPane.showMessageDialog(null, " # This is an encryption and decrypting device there's no output visible to the user by default  \n  # By default the output is directly copied into your clipboard. \n # You can change settings by clicking on settings logo. \n #The word must be Case-sensetive i.e... Using Capslock is Strictly discouraged! \n https://github.io/hellforgod ","Info",JOptionPane.INFORMATION_MESSAGE);
			}
		});
		info.setIcon(new ImageIcon(Main.class.getResource("/icon/icons8-question-mark-50.png")));
		info.setBounds(725, 13, 48, 50);
		info.setOpaque(false);
		info.setContentAreaFilled(false);
		info.setBorderPainted(false);
		info.setFocusable(false);
		frame.getContentPane().add(info);
		
	
		JButton decrypt = new JButton("Decrypt");
		decrypt.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				try {
					if(valid == true) {
						DateTimeFormatter dtf = DateTimeFormatter.ofPattern("dd"); 
						 LocalDateTime now = LocalDateTime.now();  
						  int twofour= Integer.parseInt(dtf.format(now));
					      twofour = twofour%10;
					      int qo , qq; 
							qo = Integer.parseInt(d.getText(),16);
							qq = qo;
							int [] jfk = new int[10];
							 int b = 0;
							   while (qo > 0) {
							     
							       jfk[b] = qo%10;
							       qo = qo / 10;
							       b++;
							   }
							String loc = System.getProperty("user.home");
							File file = new File(loc+"\\sc.txt");
							FileWriter wri = new FileWriter(file,true);

						char a[] = raw.getText().toCharArray();
						int c ,shift;

						shift = jfk[twofour];
						for(int size = 0;size<a.length;size++) {
							c = a[size];
							if(c<=96 || c >= 123) {
								wri.write((char)c);
							}
							if(a[size] > 96 &&a[size] < 123) {
								c = c-shift;
								if(c<97) {
									c =a[size]+26-shift;
								
								}
								else {
								
								}
							wri.write((char)c);
							}
							else {
							}	
							
						}
						wri.close();
						Scanner sc = new Scanner(file);
						last = sc.nextLine();
				
						sc.close();		
						file.delete();
						if(show == true) {
							cpy1.setVisible(true);	
							ans.setText(last);
							cpy1.addActionListener(new ActionListener() {
								public void actionPerformed(ActionEvent e) {
									Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
								}
							});
							frame.getContentPane().add(cpy1);
							}
						else {
							Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
						}

					      
					
					}
					else {
					if(eww == true) {
						int qo , qq; 
						qo = Integer.parseInt(d.getText(),16);
						qq = qo;
						int [] jfk = new int[10];
						 int b = 0;
						   while (qo > 0) {
						     
						       jfk[b] = qo%10;
						       qo = qo / 10;
						       b++;
						   }
						String loc = System.getProperty("user.home");
						File file = new File(loc+"\\sc.txt");
						FileWriter wri = new FileWriter(file,true);

					char a[] = raw.getText().toCharArray();
					int c ,shift;

					shift = jfk[3];
					for(int size = 0;size<a.length;size++) {
						c = a[size];
						if(c<=96 || c >= 123) {
							wri.write((char)c);
						}
						if(a[size] > 96 &&a[size] < 123) {
							c = c-shift;
							if(c<97) {
								c =a[size]+26-shift;
							
							}
							else {
							
							}
						wri.write((char)c);
						}
						else {
						}	
						
					}
					wri.close();
					Scanner sc = new Scanner(file);
					last = sc.nextLine();
			
					sc.close();		
					file.delete();
					if(show == true) {
						cpy1.setVisible(true);	
						ans.setText(last);
						cpy1.addActionListener(new ActionListener() {
							public void actionPerformed(ActionEvent e) {
								Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
							}
						});
						frame.getContentPane().add(cpy1);
						}
					else {
						Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
					}
					
					}
					else {
					
					String loc = System.getProperty("user.home");
					File file = new File(loc+"\\sc.txt");
					FileWriter wri = new FileWriter(file,true);

				char a[] = raw.getText().toCharArray();
				int c ,shift;

				shift = Integer.parseInt(d.getText());
				for(int size = 0;size<a.length;size++) {
					c = a[size];
					if(c<=96 || c >= 123) {
						wri.write((char)c);
					}
					if(a[size] > 96 &&a[size] < 123) {
						c = c-shift;
						if(c<97) {
							c =a[size]+26-shift;
						
						}
						else {
						
						}
					wri.write((char)c);
					}
					else {
					}	
					
				}
				wri.close();
				Scanner sc = new Scanner(file);
				last = sc.nextLine();
		
				sc.close();		
				file.delete();
				if(show == true) {
					cpy1.setVisible(true);	
					ans.setText(last);
					cpy1.addActionListener(new ActionListener() {
						public void actionPerformed(ActionEvent e) {
							Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
						}
					});
					frame.getContentPane().add(cpy1);
					}
				else {
					Toolkit.getDefaultToolkit().getSystemClipboard().setContents(new StringSelection(last),null);
				}
					}
				}
				}
				catch (Exception ex) {
			    ex.printStackTrace();
					
				}
			}
				
	});
		decrypt.setForeground(Color.WHITE);
		decrypt.setFont(new Font("Arial", Font.BOLD, 25));
		decrypt.setBounds(402, 298, 140, 39);
		decrypt.setOpaque(false);
		decrypt.setContentAreaFilled(false);
		decrypt.setBorderPainted(false);
		decrypt.setFocusable(false);
		frame.getContentPane().add(decrypt);
		
	

		
	}
}
		
