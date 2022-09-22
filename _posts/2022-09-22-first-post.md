---
title: "My first post"
layout: post
---

As the title suggests, this is my first post! In this feed I'll post updates on projects I'm working on, write a short summary of papers that have been published or post my thoughts on topics that I know something about.

For instance, I'm currently improving my Python skills by starting from the absolute basics using (Codility)[https://app.codility.com/programmers/lessons/1-iterations/]. Even though I've used Python in much more advanced applications, some lessons are actually quite challenging. Whenever I've completed a lesson, I'll push the code to my (GitHub)[https://github.com/DWvanderMeer/codility].

You can find the code from today's lesson (here)[https://github.com/DWvanderMeer/codility/blob/main/L4_MaxCounters.py]:

{% highlight ruby %}
def solution(N, A):
    res = [0 for i in range(N)]
    for i in range(len(A)):
        if A[i] <= N:
            res[A[i]-1] = res[A[i]-1]+1
        elif A[i] == N+1:
            res = [max(res) for j in range(N)]
    return(res)
{% endhighlight %}

