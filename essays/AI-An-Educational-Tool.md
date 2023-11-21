---
layout: essay
type: essay
title: "AI: The Latest Educational Tool"
# All dates must be YYYY-MM-DD format!
date: 2023-11-20
published: true
labels:
  - Software Engineering
  - Artifical Intelligence
  - Education
---
## Introduction:

The use of AI by students is seen by many as “cheating” due to its ability to produce answers for most if not all educational material. In reality AI is simply a new tool for students to use to further their education, especially in the case of Software Engineering. Calculators, like AI, were once seen by teachers as a tool that would disrupt a student's education. Today the use of calculators is the standard and its use is mandated on many tests. Though the use of AI is looked down upon by Universities, it will undoubtedly become an essential part of education in the near future.

My instructors this semester have been gracious enough to allow the use of AI for their courses, though obviously within reason (hence why I am writing this essay). Through my use of Open AI’s chatGPT and GitHub Co-Pilot in combination with the lessons of my instructor, in a matter of months I have been able to learn many concepts of web development. There were many times where I was confused about how to implement a given concept, and rather than scouring through documentation for hours, I was able to find answers to many of my questions instantly via my use of AI. 

## Personal Experience with AI:
Here are some examples of how I have used AI in ICS 314 thus far:

### 1. Experience WODs
Experience WODs are essentially timed homework in which you create a small program based on the provided instructions. I used AI on many of these, one in particular being E31: BrowserHistory2. In the experience I was required to add CSS styles to a HTML file, Upon creating the style.css file GitHub Copilot automatically provided me with some standard css definitions. While attempting to alter them to better fit the assignments requirements, Copilot also generated exactly what I had intended to do, this saved me a lot of time to double check everything and allowed me to finish the WOD well within the allotted time.

### 2. In-class Practice WODs
In-class Practice WODs work exactly the same as the Experience WODs except they are not graded and are completed in person with only one attempt allowed. At first I attempted these without using AI, but eventually found their use to be crucial. Though they did not affect my grade in the class, I found that practicing what prompts to use in chatGPT to produce what I was looking for to be very helpful, especially when it came time to do the graded in-class WODs. 

### 3. In-class WODs
For the In-class WODs I took very little chances, relying on chatGPT the second I found myself not knowing what to do next. A perfect example of this were any of the WODs pertaining to Javascript’s underscore library. I really struggled to understand which function to use for a given task. My solution was asking chatGPT: “Using the underscore library do <insert task to be done>” , and in seconds it provided me with code that did exactly what the WOD asked. Admittedly my personal knowledge of the underscore library at the time was not sufficient to pass. However, through chatGPTs explanation (and further research) I was able to develop a good understanding of the concepts. 

### 4. Essays
While I have never used AI to explicitly write an essay for me. I have asked chatGPT to generate an outline of an essay based on a given topic. I then found credible sources and wrote my essay by more or less following the structure of the AI generated outline. I believe this is an ethical way of using AI to assist in the writing process as it simply provides you with a launching off point for writing one's own essay. 

### 5. Final project
For my group's final project we created an AI chat-bot that answers UH specific information technology service (ITS) related questions based on articles from the UH ITS FAQ. This required us to work with OpenAI’s API, as well as the vector database platform Pinecone. Initially knowing nothing about how to work with either of these I asked chatGPT for information. Surprisingly it provided very little knowledge as many of the frameworks and services were created/updated after chatGPT’s cut off date of January 2022. Thus I was forced to dig through OpenAI’s documentation to figure out many of the problems I was running into. 
 
### 6. Learning a concept / tutorial
In another of my classes ICS 390 I am an ATA of an ICS 211 lab. I often mind self needing a refresher on many of the courses concepts such as binary search trees or heaps. With chatGPT I can simply write a prompt such as “What is a binary search tree?” or “Create a binary search tree in Java”, and am provided with a concise breakdown of the concept as well as how to implement it. This has proven very helpful and I often recommend the students to ask chatGPT similar questions if they are still struggling. 

### 7. Answering a question in class or in Discord
I have never used AI to answer a question in class or in Discord simply because I have never answered a question I did not already know the answer to. I am sure chatGPT is very useful in answering these questions as I often ask the AI questions myself. However I feel if I had to ask chatGPT for the answer I likely don't have the proper knowledge to effectively answer the question. 

### 8. Asking or answering a smart-question
I have also never used AI to answer a smart-question posted in the discord channel simply because I assume the poster has already attempted to ask chatGPT their question before asking. Thinking about it now, it would have been smarter to double check this before looking into their problems based on some of the “smart” questions people have asked. 

### 9. Coding example 
Referring to the Learning a concept / tutorial section of this essay where I asked chatGPT to “Create a binary search tree in Java”. The AI returned the following:
```
class Node {
    int key;
    Node left, right;

    public Node(int item) {
        key = item;
        left = right = null;
    }
}

public class BinarySearchTree {
    Node root;

    public BinarySearchTree() {
        root = null;
    }

    // Insert a key into the BST
    public void insert(int key) {
        root = insertRec(root, key);
    }

    // A recursive function to insert a key into BST
    private Node insertRec(Node root, int key) {
        // If the tree is empty, create a new node
        if (root == null) {
            root = new Node(key);
            return root;
        }

        // Otherwise, recur down the tree
        if (key < root.key)
            root.left = insertRec(root.left, key);
        else if (key > root.key)
            root.right = insertRec(root.right, key);

        // Return the (unchanged) node pointer
        return root;
    }

    // Inorder traversal of the BST
    public void inorder() {
        inorderRec(root);
    }

    // A utility function to do inorder traversal of BST
    private void inorderRec(Node root) {
        if (root != null) {
            inorderRec(root.left);
            System.out.print(root.key + " ");
            inorderRec(root.right);
        }
    }

    public static void main(String[] args) {
        BinarySearchTree tree = new BinarySearchTree();

        // Insert keys
        tree.insert(50);
        tree.insert(30);
        tree.insert(20);
        tree.insert(40);
        tree.insert(70);
        tree.insert(60);
        tree.insert(80);

        // Print inorder traversal
        System.out.println("Inorder traversal:");
        tree.inorder();
    }
}

```
As you can see chatGPT provides an excellent implementation of a binary search tree with comments that explain what each section of code does. 

### 10. Explaining code
Oftentimes while writing code GitHub CoPilot will generate code to do what it expects you want to achieve, because of this I have sometimes found myself with functional code that I don’t fully understand. This is easily remedied by asking chatGPT to explain what this code is doing, and how it works. Just recently I was trying to update the value of a field of a document within a MongoDB collection, CoPilot generated code that used the $inc operator. Not knowing what it was I asked chatGPT, it explained how the operator is used to increment the value of the specified field and suddenly it all made sense to me. 

### 11. Writing code
GitHub CoPilot has probably written a third of the code I’ve used in my programs for this course. Its ability to generate code that achieves exactly what you want it to do is uncanny, and has quickly become essential to my productivity. 

### 12. Documenting code
In addition to writing code, GitHub CoPilot also creates documentation for any code it or you wrote, simply start to write a comment and it will do the rest. 

### 13. Quality assurance 
I have never used AI to help solve errors in my code as I feel figuring out what exactly these issues are is where one learns the most. 

### 14. Other uses in ICS 314 not listed
I think it is safe to say I have covered all the way in which I’ve used AI in ICS 314.

##  Impact on Learning and Understanding:
Incorporating the use of AI into my learning experience has greatly improved my problem-solving abilities. With a simple prompt into chatGPT I am able to learn about or even straight up solve any problem I am facing. However, it is undeniable that if used irresponsibly, AI has the potential to completely derail one's comprehension of core concepts. At the end of the day this boils down to whether someone wishes to learn, or simply pass a course. AI provides students with either possibility, and it is up to the individual users to determine whether they want to absorb the information it provides, or merely copy and paste the answers. In my case, I believe that the use of AI has only enhanced my understanding of software engineering concepts.  

## Practical Applications:
The use of AI has many practical applications outside the realm of education. Just recently I was participating in the Hawaii Annual Coding Challenge (HACC) and made great use of GitHub CoPilot when developing for my team’s program. Furthermore, GitHub conducted a survey on AI’s impact on the developer experience and found that 92% of the developers in their study are using AI at work. If such a staggering majority of working developers are using these tools I think it is safe to say that there is no shortage of practical applications of AI.

## Challenges and Opportunities:
The only challenge I’ve encountered in the use of AI within this course would be retrieving any information created after January 2022 from chatGPT. However, I believe this will soon no longer be an issue with chatGPT 4.0 now being connected to the internet. As for potential opportunities for further integration of AI in software engineering education I believe the possibilities are endless.

## Comparative Analysis:
Without a shadow of a doubt the use of AI has enabled me to learn countless practical skills and their associated software engineering concepts. However, when compared to my experience learning the basics in ICS 111 and 211 without AI, my ability to retain information has definitely decreased. I believe that this is simply due to solutions being much more easily accessible through the use of AI. No longer do I find myself stumped for days at a time trying to figure out a concept. Instead I turn to the help of AI tools like chatGPT or GitHub CoPilot and figure out solutions in at most a matter of hours. Sure I no longer get this information pounded into my brain, but one could argue that with the ease of access to this information via AI, what reason is there to? 

## Future Considerations:
I believe that AI will play a huge role in future software engineering education. Perhaps all courses will eventually permit the use of AI. For this to be the case however, a more education centered AI application will have to be made, that does not simply give the answers to students, but instead guides them to figuring it out themselves. 

## Conclusion:
To conclude, AI tools such as ChatGPT and GitHub CoPilot have proven invaluable to me this semester, and likely will continue to be for the foreseeable future. AI’s role in educational and professional environments will continue to grow, and it is important that the curriculum taught to students grow with it. Yes, AI currently has the potential to ruin a students education, but that is why it is crucial for them to be taught why it is valuable for them to learn beyond simply copying and pasting code. 
