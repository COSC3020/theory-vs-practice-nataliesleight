# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  Three reasons that asymptotic analysis couuld be misleading are:

  1. If it is using Big O or Big Omega, the upper and lower bounds can be just that. The actual perforance can be anywhere within the one sided bounds.
  2. Asymptotic analysis does not account for differences in hardwares and softwares.
  3. Because asymptotic analysis analyzes the asymptotes (hence the name), "smaller" input sizes may be more greatly affected by the parts of an equation 
     that become obsolete as the input approaches infinity.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  I would guess that the time it would take would be around 8-50 seconds. I solved for 50 seconds by simply multiplying the
  original time by 10, as the input size it 10 times larger than the origianl input. For 8, I used the time complexity of
  $O(log_2 n)$ to solve for the time complexities of input size 1,000 (~ 9.97) and input size 10,000 (~ 13.28). I then divided
  them by each other to get a proportion of the 10,000 size being greater than the 1,000 size by 50%. Next I multipled the original
  time by 1.5 (to make it 50% larger) to get 7.5 seconds, rounding up to 8 for sake of simplicity. 

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  Three reasons why the actual performance may have been different:

  1. The two tests could have been run on different machines.
  2. More applications could have been running in the background during the second test.
  3. The computer may be overheating (for external reasons such as dust build-up) during the second run, resulting in the computer slowing down to produce less heat to avoid damage.
  
Add your answers to this markdown file.

### Sources:

I used the examples we covered in class on Thursday 2/20. I used this site to look into overheating: https://computronixusa.com/what-causes-a-computer-to-run-slow/ 

“I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.” - Natalie Sleight
