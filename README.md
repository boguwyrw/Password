/* # Password
Small project in Java from postgraduate studies */

package Pass;

import java.util.Scanner;

public class Main {
    public static final String PASSWORD = "quwerty";

    public static void main(String[] args) {
        String pass;
        boolean isPassOK = false;
        int MAX_PASS = 3;
        int passCount = 0;

        do {

            System.out.println("Enter the password: ");
            Scanner scanner = new Scanner(System.in);
            pass = scanner.next();
            if (pass.equals(PASSWORD))
            {
                System.out.println("Password is correct. Welcome user.");
                isPassOK = true;
            }
            else{
                System.out.println("Wrong password");
            }
                passCount++;
            }
            while (!isPassOK && passCount < MAX_PASS) ;
        }
    }
