Download Link: https://assignmentchef.com/product/solved-cs2040s-sort-of-sorting
<br>
Sorting is a really fun way to order things. In particular sorting strings is particularly interesting since there are many ways to order them. For example there is the <em>lexicographic </em>ordering which is the default String comparison that Java does. In lexicographic ordering, given two strings <em>a </em>= <em>a</em><sub>1</sub><em>a</em><sub>2</sub><em>a</em><sub>3 </sub><em>…a<sub>m </sub></em>and <em>b </em>= <em>b</em><sub>1</sub><em>b</em><sub>2</sub><em>b</em><sub>3 </sub><em>…b<sub>n</sub></em>, we say that <em>a </em>≺<em><sub>lex </sub>b </em>if any of the following are satisfied.

<ol>

 <li><em>a </em>= <em>ε</em></li>

 <li>If <em>m </em>≤ <em>n </em>and <em>a<sub>i </sub></em>≤ <em>b<sub>i </sub></em>for all <em>i </em>∈ [1<em>…m</em>]</li>

 <li>If for some integer <em>k </em>where <em>k </em>≤ <em>m,n</em>, and <em>k </em>≥ 1, for all <em>i </em>∈ [1<em>…k </em>− 1] <em>a<sub>i </sub></em>= <em>b<sub>i </sub></em>and <em>a<sub>k </sub></em>6= <em>b<sub>k </sub></em>and in fact <em>a<sub>k </sub>&lt; b<sub>k </sub></em>in terms of character comparsion.</li>

</ol>

However, sorting the normal way is boring. Given a class list, you are going to label the tables with the first two letters of each student’s name. You would also like these two letter names to be in running order (i.e. in sorted order).

In addition to this, you would like to minimise the number of swaps within the class list that you require to do. Hence you would like your sorting algorithm to be <strong>stable</strong>. Recall that a sorting algorithm is stable if given two objects <em>a </em>and <em>b</em>, if <em>a </em>= <em>b </em>based on the comparison used by the sorting algorithm and <em>a </em>appears before <em>b </em>in the original list, then <em>a </em>will appear before <em>b </em>in the sorted list.

You are given the class file Sorter.java, as shown below: public class Sorter {

public static void sortStrings(String[] arr) {

// TODO: implement your sorting function here }

}

The function sortStrings(String[] arr) takes in an array of strings and performs a sort <strong>in place </strong>on the given array. You may refer to SorterTest.java to see how this method is called.

You may find implementing the following function to be helpful as well

public static boolean isGreaterThan(String str1, String str2) {

//your implementation here return false

}

1

which takes in two strings and outputs whether str1≺str2. based on what ordering you wish ≺ to represent. Use the tests in SorterTest.java to test your implementation against sample tests. When you are done, only upload the completed file Sorter.java to Coursemology.