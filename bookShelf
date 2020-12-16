package readxml_jdomandxpath;

import java.io.File;
import org.jdom2.Attribute;
import org.jdom2.Document;
import org.jdom2.Element;
import org.jdom2.JDOMException;
import org.jdom2.filter.Filters;
import org.jdom2.input.SAXBuilder;
import org.jdom2.xpath.XPathExpression;
import org.jdom2.xpath.XPathFactory;
import java.io.IOException;
import java.io.InputStream;
import java.util.List;

public class bookShelf {
    
    File xmlFile;
    SAXBuilder builder;
    Document doc;
    XPathFactory xpath;
    XPathExpression expr;
    List<Element> books;
    Element e;
    
    initialVars var = new initialVars();
    
    public bookShelf(String xmlPath) throws IOException, JDOMException {
        this.xmlFile = new File(""); //the file path
        this.builder = new SAXBuilder();
        this.doc = builder.build(xmlFile);
        this.xpath = XPathFactory.instance();
        
    }
    
    public bookShelf() throws JDOMException, IOException{
        InputStream in = bookShelf.class.getResourceAsStream(""); //the file path
        SAXBuilder builder = new SAXBuilder();
        Document document = builder.build(in);
        XPathFactory xpath = XPathFactory.instance();
        XPathExpression<Element> expr = xpath.compile("//bookshelf/book", Filters.element());
        List<Element> courses = expr.evaluate(document);
        for (Element course : courses){
            System.out.println("   " + course.getValue().trim());
        }

    }
    
    public void selectElements() throws JDOMException, IOException{
        InputStream in = bookShelf.class.getResourceAsStream(""); //the file path
        SAXBuilder builder = new SAXBuilder();
        Document document = builder.build(in);
        XPathFactory xpath = XPathFactory.instance();
        XPathExpression<Element> expr = xpath.compile("//bookshelf/book", Filters.element());
        List<Element> courses = expr.evaluate(document);
        for (Element course : courses){
            System.out.println("   " + course.getValue().trim());
        }
    }
    
    
    /*public void selectElements(){
        this.expr = xpath.compile("\\bookshelf\\book", Filters.element());
        this.books = expr.evaluate(doc);
        for (Element book : this.books){
            //System.out.printf("%s\t" , book.getValue());
            System.out.println(e.getAttributeValue("id")+" "+e.getValue());
            String name = e.getValue();
            switch(e.getAttributeValue("id")){
                case "1001": var.setAuthor(name); break;
                case "2001": var.setAuthor(name); break;
            }
        }
        this.expr = xpath.compile("/bookshelf/book/bookname", Filters.element());
        this.books = expr.evaluate(doc);
        var.setBookName(e.getValue());

    }*/

}
