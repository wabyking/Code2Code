# Code2Code

## Motivation

>This  repository ties to translate a source code into a target one, including Python/JAVA/C++/JS.

## Example
We have a c++ source code like
<pre><
#include<iostream>
using namespace tsd;
int main()
{
   int m=0;
   while(cin>>m)  
        cout<<m+1;
}
</pre>
We would get a target Python code like
<pre>
<code>
  while(m=input())
      print(int(m)+1)
</code>  
</pre>
In order to reduce the complexity of this problem, exception check is not necessary for us.


Firstly, we should prepare well-organized parallel codes. Then we will provide a rule-base baseline and seq2seq baseline. 

## Evaluation

The evaluation is based on these three parts

+ Rouge/Mentor/Belu metrics in machine translation
+ Whether the generated code is runable
+ Whether the code keeps coherent with  the source code.

## RL-based consideration
If possible a RL-based language model as a agent is welcome for this task, due to the rewards can be well-defined, e.g. whether the compiling process has no errors or the output is coherent as the source language with a same input.


## Expectation

It can be excepted that the Machine Agent could have a better performance over human in this task.

## Contributor
-	[@WangLilian](https://github.com/WangLilian)
-	[@Garethwu](https://github.com/noline)


