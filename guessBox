import java.awt.*;
import java.awt.event.*;
import javax.swing.*;
import java.util.*;

public class guessBox extends JFrame{
	//insert the images, panel, button, and labels
	ImageIcon picture0 = new ImageIcon("8.png");
	ImageIcon picture1 = new ImageIcon("4.png");
	ImageIcon picture2 = new ImageIcon("7.png");
	ImageIcon picture3 = new ImageIcon("1.png");
	ImageIcon picture4 = new ImageIcon("5.png");
	
	JLabel start;
	
	JPanel initial = new JPanel();
	JPanel Ready = new JPanel();
	JPanel Again = new JPanel();
	JPanel change = new JPanel(new GridLayout(1,3,20,20));
	
	JButton jbtReady = new JButton("Start!");
	JButton jbtAgain = new JButton("Again!");
	
	JButton jbtChoose1 = new JButton("Choose");
	JButton jbtChoose2 = new JButton("Choose");
	JButton jbtChoose3 = new JButton("Choose");
	
	int times= 0;
	int score = 0;
	JTextField jtfScore = new JTextField(5);
	
	guessBox(){
		ImageIcon[] pic = new ImageIcon[3];
		pic[0] = picture2;
		pic[1] = picture3;
		pic[2] = picture4;
		//panel "initial" is used to show the picture
		start = new JLabel(picture0);
		initial.add(start);
		
		jtfScore.setText("Score: " + String.format("%d",score));
		
		Ready.add(jbtReady,new FlowLayout(FlowLayout.CENTER));
		Again.add(jbtAgain,new FlowLayout(FlowLayout.CENTER));
		
		change.add(jbtChoose1);
		change.add(jbtChoose2);
		change.add(jbtChoose3);
		
		add(jtfScore, BorderLayout.NORTH);
		add(initial, BorderLayout.CENTER);
		add(Ready, BorderLayout.SOUTH);
		
		jbtAgain.addActionListener(new ActionListener(){
			@Override
			public void actionPerformed(ActionEvent e){
				
				score = 0;
				times = 0;
				//restart the game
				jtfScore.setText("Score: " + String.format("%d",score) + "  Times: " + String.format("%d",times));
				start.setIcon(picture0);
				
				getContentPane().remove(Again);
				getContentPane().add(Ready, BorderLayout.SOUTH);
				getContentPane().validate();
				getContentPane().repaint();
			}
		});
		
		jbtReady.addActionListener(new ActionListener(){
			@Override
			public void actionPerformed(ActionEvent e){
				//start the game
				jtfScore.setText("Score: " + String.format("%d",score) + "  Times: " + String.format("%d",times));
				start.setIcon(picture1);
				
				getContentPane().remove(Ready);
				getContentPane().add(change, BorderLayout.SOUTH);
				getContentPane().validate();
				getContentPane().repaint();
			}
		});
		
		jbtChoose1.addActionListener(new ActionListener(){
			@Override
			public void actionPerformed(ActionEvent e){
				
				int i = (int)(Math.random() * 3) ;
				
				times++;
				
				if(i == 0)
					score+=10;
				else{
					if(score >= 5)
						score-=5;
				}
				
				jtfScore.setText("Score: " + String.format("%d",score) + "  Times: " + String.format("%d",times));
				start.setIcon(pic[i]);
		
				initial.repaint();
				
				if(times == 10){
					getContentPane().remove(change);
					getContentPane().add(Again, BorderLayout.SOUTH);
					getContentPane().validate();
					getContentPane().repaint();
				}
				else{
					getContentPane().remove(change);
					getContentPane().add(Ready, BorderLayout.SOUTH);
					getContentPane().validate();
					getContentPane().repaint();
				}
			}
		});
		
		jbtChoose2.addActionListener(new ActionListener(){
			@Override
			public void actionPerformed(ActionEvent e){
				
				int i = (int)(Math.random() * 3) ;
				
				times++;
				
				if(i == 1)
					score+=10;
				else{
					if(score >= 5)
						score-=5;
				}
				
				jtfScore.setText("Score: " + String.format("%d",score) + "  Times: " + String.format("%d",times));
				start.setIcon(pic[i]);
		
				initial.repaint();
				
				if(times == 10){
					getContentPane().remove(change);
					getContentPane().add(Again, BorderLayout.SOUTH);
					getContentPane().validate();
					getContentPane().repaint();
				}
				else{
					getContentPane().remove(change);
					getContentPane().add(Ready, BorderLayout.SOUTH);
					getContentPane().validate();
					getContentPane().repaint();
				}
			}
		});
		
		jbtChoose3.addActionListener(new ActionListener(){
			@Override
			public void actionPerformed(ActionEvent e){
				
				int i = (int)(Math.random() * 3) ;
				
				times++;
				
				if(i == 2)
					score+=10;
				else{
					if(score >= 5)
						score-=5;
				}
				
				jtfScore.setText("Score: " + String.format("%d",score) + "  Times: " + String.format("%d",times));
				start.setIcon(pic[i]);
		
				initial.repaint();
				
				if(times == 10){
					getContentPane().remove(change);
					getContentPane().add(Again, BorderLayout.SOUTH);
					getContentPane().validate();
					getContentPane().repaint();
				}
				else{
					getContentPane().remove(change);
					getContentPane().add(Ready, BorderLayout.SOUTH);
					getContentPane().validate();
					getContentPane().repaint();
				}
			}
		});
	}

	public static void main(String[] args){
		JFrame frame = new guessBox();
		frame.setTitle("U10316033");
		frame.setLocationRelativeTo(null); // Center the frame
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frame.setSize(600, 500);
		frame.setVisible(true);
	}
}
