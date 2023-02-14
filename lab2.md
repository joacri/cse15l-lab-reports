# Lab Report 2
> Servers and Bugs

## Part 1: String Server
> The following is the code for my StringServer, which keeps track of a single string that gets added to by incoming requests.
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    String str = "";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return String.format(str);
        } else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {
                    str += parameters[1] +"\n";
                    return String.format(str);
                }
            }
            return "404 Not Found!";
        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
> The following screenshots are of me using /add-message:

> - Which methods in your code are called?
> - What are the relevant arguments to those methods, and the values of any relevant fields of the class?
> - How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

>- Which methods in your code are called?
> - What are the relevant arguments to those methods, and the values of any relevant fields of the class?
> - How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
---
## Part 2: Bugs
> 
---
## Part 3: Learning
> One of the things that I fou
