I have some code here check it out:
import javax.swing.JFrame;
import java.awt.Rectangle;
import javax.swing.JComponent;
import java.awt.Graphics;
import java.awt.Graphics2D;
import java.awt.Color;
import java.awt.geom.RoundRectangle2D;

public class ThankYou {
  public static void main(String[] args) {
    JFrame lets = new JFrame(); lets.setSize(1280,960);
    lets.setTitle("Going for 3D");
    lets.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    lets.setVisible(true);

    class Block extends JComponent {
        public void paintComponent(Graphics g) {
            Graphics2D g2 = (Graphics2D) g;

            g.setColor(new Color(160, 82, 45));
            g.fillRect(10, 10, 100, 50);
            int[] aa = {110, 140, 140, 110};
            int[] bb = {10, 30, 80, 60};
            g.fillPolygon(aa, bb, 4);
            int[] xx = {10, 110, 140, 30};
            int[] yy = {60, 60, 80, 80};
            g.fillPolygon(xx, yy, 4);
            g.setColor(new Color(255,255,255));
            g.fillRect(45, 10, 20, 50);
            int[] me = {45, 65, 95, 75};
            int[] iam = {60, 60, 80, 80};
            g.fillPolygon(me, iam, 4);
            g.setColor(new Color(150, 72, 35));
            int[] aaa = {110, 140, 140, 110};
            int[] bbb = {10, 30, 80, 60};
            g.fillPolygon(aaa, bbb, 4);
            int[] xxx = {10, 110, 140, 30};
            int[] yyy = {60, 60, 80, 80};
            g.fillPolygon(xxx, yyy, 4);
            g.setColor(new Color(245,245,245));
            int[] meh = {45, 65, 95, 75};
            int[] iham = {60, 60, 80, 80};
            g.fillPolygon(meh, iham, 4);
          
        }
    }

    lets.add(new Block());
 }
}
Its a lot, I know
