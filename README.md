# Algorithms
## Part one: Fundamentals
> The objective of this book is to study a broad variety of important and useful algorithms--methods for solving problems that are suited for computer implementation. Algorithms go hand in hand with data structures--schemes for organizing data that leave them amendable to efficient processing by an algorithm. This chapter introduces our basic tools that we need to study algorithms and data structures.
>> First, we introduce our basic programming model. All of our programs are implemented using a small subset of the java programming model plus a few of our own libraries for input/output and for statistical calculations. **SECTION 1.1 is a summary of language constructs, features, and libraries that we use in this book.**  
Next, we emphasize data abstraction, where we define abstract data types (ADTs) in the services of modular pogramming. **In SECTION 1.2 we introduce the process of implementing an ADT in Java, by specifying an applications programming interfaces (API) and then using the Java class mechanism to develop an implementation for use in client code.**  
As important and useful examples, we next consider three fundamentals ADTs: the bag, the queue, and the stack. **SECTION 1.3 describes APIs and implementations of bags, queues, and stack using arrays, resizing arrays, and linked lists that serve as models and starting points for algorithm implementations throughout the book.**  
Performance is a central consideration in the study of algorithms. **SECTION 1.4 describes our approach to analyzing algorithms performance. The basis of our approach is the scientific method: we develop hypotheses about performance, create mathmatical models, and run experiments to test them, repeating the process as necessary.**  

> we conclude with a case study where we consider solutions to a connectivity problem that uses algorithms and data structures that implement the classic *Union-find* ADT.

**Defination of Algorithms**  
>When we write a computer program, we are generally implementing a method that has been devised previously to solve some problem. This method is often independent of the paticular programming language being used--it is likely to be equally appropriate for many computers and many programming languages. It is the method, rather than the computer program itself, that specifies the step that we can take to solve the problem. The term *algorithm* is used in computer science to describe a **finite, deterministic, and effetive** problem-solving method suitable for implementation as a computer program. Algorithms are the stuff of computer science: they are central objects of study in the field.  
We can define an algorithm by describing a procedure for solving a problem in a natural language, or by writing a computer program that implements the procedure.

> Here is a example as shown at below for Euclid's(欧几里得) algorithm for finding the greatest common divisor of two numbers, a variant of which was devised over 2300 years ago. 

```java
//Euclid's algorithm
public static int gcd(int p, int q){
    if (q == 0) return p;
    int r = p % q;
    return gcd(q, r);
}
```

**Algorithms and data structures**

> In this book, we use computer programs to describe algorithms. One important reason for doing so is that it makes easier the task of checking whether they are finite, deterministic, and effective, as required. But it is also important to recognize that a program in a particular language is just one way to express an algorithm. The fact that many of the algorithms in this book have been expressed in multiple programming languages over the past several decades reinforces the idea that each algorithm is a method suitable for implementation on any computer in any programming language.  
Most algorithms of interest involve organizing the data involved in the computation. Such organization leads to *data structures*, which also are central objects of study in computer science. Algorithms and data structures go hand in hand. *In this book we take the view that data structures exists as the byproducts or end products of algorithms and that we must therefore study them in order to understand the algorithms.* **Simple algorithms can give rise to complicated data structures and, conversely, complicated algorithms can use simple data structures.** We shall study the properties of many data structures in this book; 

**Why should we learn Algorithms?**

> when we use  computer to help us solve a problem, we typically are faced with a number of possible approaches. For small problems, it hardly matters which approach we use, as long as we have one that correctly solves the problem. **For huge problems, however, we quickly become motivated to devise methods that use time and space efficiently.**  
***The primary reason to learn about algorithms is that this discipline gives us the potential to reap huge savings, even to the point of enabling us to do tasks that would otherwise be impossible.*** In an application where we are processing millions of objects, it is not unusual to be able to make a program millions of times faster by using a well-designed algorithm. We shall see such examples on numerous occasions throughout the book. By contrast, investing additional  money or time to buy and install a new computer holds the potential for speeding up a program by perhaps a factor of only 10 or 100. Careful algorithm design is an extremely effective part of the process of solving a huge problem, whatever the applications area.  
The sharing of programs in computer systems is becoming more widespread, so although we might expect to have to implement only a small fraction of them. For example, the Java libraries contain implementations of a host of fundmental algorithms. However, implementing simple versions of basic algorithms helps us to understand them better and thus to more effictively use and tune advanced versions from a library. More important, the opportunity to reimplement basic algorithms arises frequently. The primary reason to do so is that we are faced, all too often, with completely new computing environments with new features that old implementations may not use to best advantage. In this book, we concentrate on the simplest reasonable implementations of the best algorithms. We do pay careful attention to coding the critical parts of the algorithms, and take pains to note where low-level optimization effort could be most beneficial.

**Summary of topics**  
> As a overview, we describe the major parts of the book, giving specific topics covered and an indication of our general orientation toward the material. This set of topics is intended to touch on as many fundamental algorithms as possible. Some of the areas covered are core computer-science areas that we study in depth to learn basic algorithms of wide applicability. Other algorithms that we discuss are from advanced fields of study within computer science and related fields. The algorithms that we consider are the products of decades of research and development and continue to play an essential role in the ever-expanding applications of computation.  
Fundamentals (chapter 1) in the context of this book are the basic principles and methodology that we use to implement, analyse, and compare algorithms. We consider our Java programming model, data abstraction, basic data structures, abstract data types for collections, methods of analyzing algorithm performance, and a case study.  
sorting (chapter 2) for rearranging arrays in order are of fundamental importance. We consider a variety of algorithms in considerable depth, including insertion sort, shell sort, quick sort, mergesort, and heapsort. We also enconter algorithms for several related problems, including priorith queues, selection, and merging. Many of these algorithms will find application as the basis for other algorithms later in the book.  
Searching (chapter 3) for finding specific items among large collections of items are also of fundamental importance. We discuss basic and advanced methods for searching, including binary search trees, balanced search trees, and hashing. We note relationships among these methods and compare performance.   
Graphs (chapter 4) are sets of objects and connections, possibly with weights and orientation. Object are useful models for a vast number of difficult and important problems, and the design of algorithms for processing graphs is a major field of study. We consider depth-first search, breadth-first search, connectivity problems, and several algorithms and applications, including kruskal's and prim's algorithms for finding minimum spanning tree and Dijstra's and the Bellman-Ford algorithms for solving shortest-paths problems.


