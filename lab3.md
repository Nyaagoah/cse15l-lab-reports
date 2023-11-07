Lab Report 3 
PART 1 
Buggy Code in Question 
static void reverseln Place(int[] arr) { 
for(int i = 0; i < arr.length; i += 1) { 
} 
arr[i] 
= 
arr[arr.length - i - 1]; 
} 
Failure Inducing Test 
public class Array Tests { 
@Test 
public void testReverseInPlace() { 
int[] input1 
= 
{3,2,1}; 
ArrayExamples.reverseInPlace(input1); 
assertArrayEquals(new int[]{1,2,3}, input1); 
} 
Non-Failure Inducing Test public class ArrayTests 
{ @Test 
public void testReverseInPlace() { 
int[] input1 
= 
{3}; 
ArrayExamples.reverseInPlace(input1); 
assertArrayEquals(new int[]{3}, input1); 
} 
Symptom for Faiure Inducing Test 
