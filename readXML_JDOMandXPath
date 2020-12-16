package readxml_jdomandxpath;

import java.io.IOException;
import java.util.Scanner;
import org.jdom2.JDOMException;

public class readXML_JDOMandXPath {

    public static void main(String[] args) throws IOException, JDOMException {
        String xmlPath = "/*write XML file path here*/"; // xml file path
        bookShelf books = new bookShelf(xmlPath);
        Scanner input = new Scanner(System.in);
        int choice = 0;
        
        /*System.out.println("1. Select all elements.");
        System.out.println("2. Select all attributes of element.");
        System.out.println("3. Select the second element.");
        System.out.println("4. Select element by xpath with attribute");
        
        System.out.println("Choose a number:");
        choice = input.nextInt();
        while(choice != 5){
            switch(choice){
                case 1: books.selectElements();
                case 2: ;
                case 3: ;
                case 4: ;
                case 5: break;
            }
        }*/
        
        books.selectElements();
        
    }
    
}
