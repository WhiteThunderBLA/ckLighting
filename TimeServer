import java.io.*;
import java.net.*;
import java.util.*;

        
/** * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author Tim
 */
public class TimeServer extends Thread {
    private ServerSocket rockett;
    
    public TimeServer(){
        super();
        try{
            rockett = new ServerSocket(80);
            System.out.println("time server running");
            
        } catch(IOException e){
            System.out.println("error: system could not create socket:"
                    + e.getMessage());
            System.exit(1);
        }
        
    }
    public void run(){
        Socket client = null;
        while(true){
            if (rockett == null){
                return;
                
            }
            try{
                client = rockett.accept();
                BufferedOutputStream bos = new BufferedOutputStream(
                        client.getOutputStream());
                PrintWriter os = new PrintWriter(bos, false);
                String outLine;
                Date now = new Date();
                
                os.println(now);
                os.flush();
                
                os.close();
                client.close();
                
            }catch (IOException ioe){
                System.out.println("could not connect to client: " 
                        + ioe.getMessage());
                System.exit(1);
            }
        }
    }
    public static Date relativeTime(){
        float m1;
        if 
        float theta;
        double  v1
            v1= 150000000;
            theta = theta;
            return 
        
        float m2;
    }
    public static void main (String[] args){
        TimeServer server = new TimeServer();
        server.start();
    }
}
