# Special-Stack
Input:
Stack: 18 19 29 15 16
Output: 15
Explanation:
The minimum element of the stack is 15.
 
 
 class GfG{
	public void push(int a,Stack<Integer> s)
	{
	   s.push(a);

 }

 public int pop(Stack<Integer> s)

    {

        //add code here.

        int top = s.pop();

        return top;

 }

 public int min(Stack<Integer> s)

    {

        //add code here.

        int minElement = s.peek();

        while(!s.isEmpty())

        {

            if(s.peek() < minElement)

            {

                minElement = s.peek();

            }

            s.pop();

        }

        return minElement;

 }

 public boolean isFull(Stack<Integer>s, int n)

    {

        //add code here.

        return s.size() == n;

 }

 public boolean isEmpty(Stack<Integer>s)

    {

        //add code here.

        return s.size() == 0;   

 }

}
