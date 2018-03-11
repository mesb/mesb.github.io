---
layout: post
title: A stupid Bubble Sort story
publish: true
---


Many moons ago, in the kindgom of Funge, the Queen awoke to a difficult problem that was likely to cause the collapse of her kingdom. It appears that the problem had happened in the very long past of the kingdom and the effects were catastrophic. The Kingdom's seer, Ifgah, had a dream in which their original ancestor, Baba Aboks, appeared to her and revealed to her the arrival of a severe draught and famine that will inflict the land for close to 20 consecutive years. However, Baba Aboks kindly informed Ifgah that the kingdom has 5 years to prepare for this epidemic. It was the rush ignited by this dream that directed Ifgah, in the very early mornings, to Queen Ire's chambers.

The Queen, wise as she was, understood the critical nature of this abrupt and early visit. She dimissed all formalities and asked Ifgah to do tell all there is to know. Ifgah told her the good news. Good news, for they were informed by Baba Aboks way before the catastrophe was to strike and they've got time to prepare. The Queen also understood this. Ifgah, by some stroke of extra inspiration, told the Queen that this situation presents to the kingdom a course for better understanding of the various clans. You see, Ifgah said,

<div class="org-center">
Our various tribes occupy different regions of our blessed land. Those by the waters enjoy fishing, those by the forests enjoy hunting; those by the mountains enjoy farming. To survive the famine, we shall need to gather all the food we can and preserve them for the dry days. We can therefore divide the task of growing and stocking our stores amongst the various tribes. The hunters will be in charge of the meat, the farmers in charge of the grains. The tribes of artisans and craftsmen will also repair and upgrade the structures that will accomodate our produce.

Here comes the important piece. We can document the output of each tribe and so come to some good understanding of how much each tribe can produce. Although this may bring division for the lowly minded, we can rank the tribes according to their contributions. But for the high-minded, this ranking can help your majesty's reign understand the challenges of those who produced the least, and so implement required measures for the overall developement of the kingdom.
</div>

The Queen thought deeply about this and said, "Yes! Let the various tribe leaders come to the court immediately." By the end of the meeting, the Queen and the elders had concluded that the kingdom's tribes will specialize in their various fortes and they'd all work for the emergent solution to the forthcoming draught and famine. The elders then went to their clans, relayed the information to them; all the peoples were jolly. They presented sacrifices to their gods and began working. The tribe of the scientists came up with a system for measuring the output of each tribe. They called their scale the *nene* and output was measured in *ne(s)*.

Three years and eight months later, all the tribes had done their best and their products were stored in humongous and high-tech pyramids that were repaired by the tribe of builders. These pyramids were specialized for food and resource storage. The chief mathematician, Kkaienge, recorded the output, measured in ne(s), of each tribe and presented the data to the Queen. There were 13 tribes in that kingdom and below are the various outputs presented by Kkaienge to the Queen:


(1, 234), (2, 213), (3, 382), (4, 101), (5, 382), (6, 101), (7, 737), (8, 50), (9, 10), (10, 199), (11, 366), (12, 148), (13, 80)


Kkaienge explained the format of the data to the Queen. Each measurement is represented as a pair of numbers. The first number in the pair is the tribe number(from 1 to 13 for the 13 tribes), and the second number in the pair is the actual produce in million ne(s). Hence, Tribe number 1 produced 234 million nes. Tribe number 2 produced 213 million nes; and so on.

The Queen expressed a broad smile of relief which was also aroused by her pride for her kingdom. Their majesty was amazed at the produce of her peoples. She smiled some more and then asked Kkaienge:

"I see you and all our brothers and sisters have done wonderful jobs.
You, Kkaienge, have made a wonderful contribution by capturing this information and presenting it to us in this format. But, Ifgah originally proposed that we rank our tribes according to the total produce they contributed. I understand that for now you've arranged the information and ranked them naturally by the birth order or age of our tribes. Can you please rearrange them according to the amount of produce contributed? I'd love to see a line of the tribes such that the tribe with the smallest output will be in the first position of this lineup, the tribe with the next smallest produce will be on position 2, and the tribe with the largest produce will be at the last position of the lineup."

Kkaienge, a scientist by heart, was very excited by this new challenge. It had never arisen in their kingdom. To me and you, the task is as simple as reordering the information in ascending order. In other words, Kkaienge has been tasked with sorting the produce of the tribes in ascending order. This, now simple, problem thus appeared for the first time in this kingdom and Kkaienge and his fellow scientists had the opportunity to try to solve it. Kkaienge charged directly for the mountains, were he took a retreat that lasted 1 week. During that period, Kkaienge ate nothing but honey and he drank from a spring called the "waters of Babas". During this period, Kkaienge conveived about 20 different ways of solving this problem with the assistance of the gods. He went back to the kingdom and assembled some colleagues so that they could implement the techniques.

The Queen heard Kkaienge was back. Queen Ire, as it happened, had a knack for mathematics and science. She summonded Kkaienge and requested that Kkaienge and his team should come and solve the problem in her court so that she too can watch. She asked Kkaienge if he had any names for the techniques he would be using. Kkaienge resonded, "My Queen, I camped at holy grounds on our blessed Mt. Ipamut and I was blessed by our gods with techniques for rearranging our data. The gods said that what we are trying to do is called 'SORTING'." The Queen was mesmerized by this announcement. "Sorting," she repeated to herself. "Oh! So you have to sort the the data you collected in ascending order. Now I see!", the Queen uttered. Kkaienge continued to narrate stories of his retreat in the mountains and said the gods first taught him a technique called "Bubble Sort", then they taught him "Insertion Sort,", then "Selection Sort"; then heapsort; The Queen was already getting dizzy from immense excited.

The Queen blurted out, "Bubble Sort!" That's a funny name. Tell me about that one. "Give me as much details as you can, tell me what the gods taught you, wise Kkaienge, so that I can share in the beauty of knowledge from our gods."

The wise Kkaienge was awed by the enthusiasm of their Queen. He then said the algorithm was taught to him in the form of a story, where their gods performed the act of sorting using bubble sort so that Kkaienge could learn from the practicality of the gods.

Kkaienge began his story:

Oh wise gods of our great kindgom
Sing to us again
And tell us the steps
Of the Bubble Sort procedure
With words simple and clear,
Reveal to us this great activity

The gods first told me the word
That captures all such activities
Is known as "ALGORITHM"
An ALGORITHM is the sequence
Of steps that are involved in transforming
A given set of elements
To a desired set of results

The Bubble Sort algorithm, Kkaienge said, involves 2 key players who work together to rearrange the a lineup of entities to be sorted. These entities are also called elements. The elements form a lineup of elements, each element at a position that has a unique number. The first element is at position 1, the next at position 2, and the lineup positions extend until the last position, which the gods said is only fixed at the time of performing the actual sorting. In other words, the gods said they'd make this last position's number very general and they symbolized it by the letter \( n \). Hence, the elements to be sorted are lined up in position and in the order:

1, 2, 3, 4, &#x2026; n

That is, the numbers are lined up from 1 up to \( n \).

While I was listening to the gods, Kkaienge said, I began to get anxious and I  thanked the gods again and waited for them to continue the wonderful story. The gods then said the simple idea behind this algorithm is to divide the lineup of elements into 2 groups or regions, according to their lineup numbers. The first group will be called the \(UNSORTED \) group or region and the second group will be called the \( SORTED \) group. The players in the algorithm look for the largest element in the \( UNSORTED \) region and transport this largest element to the \( SORTED \) region. The gods also emphasized that this technique of dividing the lineup into regions is a more general technique that can be used in different ways.

Not deep into the Bubble Sort algorithm, and the Queen was in total wonderment. She exclaimed, "Oh! So can we think of the algorithm using normal ideas that we use on a daily basis?" Kkaienge replied, "It appears so my Queen." He continued to explain that the idea of regions, lineup, transportation are all normal concepts in our daily lives. The gods, however, said that there are more technical words for these concepts. For example, the lineup, as they said, can take the form of a structure called an \( ARRAY \), or generally, a \( LIST \). In the parlance of \( ARRAYS \) and \( LISTS \), the regions are called \(SUBARRAYS \) and \( SUBLISTS \). The task performer would have to create these regions and perform the steps relayed until the result, the sorted lineup or array or list, is acquired.

"Go on, dear Kkaienge, the Queen said."

"Yes my Queen."

I was instructed to divide the \( LIST \) into 2 regions, as mentioned already, and to promote the largest element from the \( UNSORTED \) region into its correct position in the sorted region.

The Bubble Sort algorithm, as they described to me, is called so because it has a funny nature of taking turns to promote the biggest element from the \( UNSORTED \) region. Each of these turns makes the largest element in the \( UNSORTED \) region to assume its correct position in the \( SORTED \) region. As a result, each turn makes the largest \( UNSORTED \) element to fly away or \( BUBBLE \) up to the correct global position. For this reason, there were 2 main spirits in the demonstration of this algorithm. The first spirit was in charge of the \( UNSORTED \) region. This spirit, in the style of Bubble Sort, searches for the largest \( UNSORTED \) element by performing strategic comparisions. The second spirit has only 1 task: this spirit simply points at the next position in which spirit 1 is to deposit the biggest \( UNSORTED \) element. As such, the great spirit that points at the next deposition point in the \( SORTED \) region changes this position at appropriate rounds of the process.

"My dear Kkaienge," the Queen interjected, "What are these rounds and how do they come about?"

My Queen, a round corresponds to a cyle of activity where a spirit performs activities that lead to the sorting of elements. For example, Spirit 2, which was called "Aboko", begins the process by pointing at the last element which is at position \( n \). While he points at position \( n \), the first spirit, aka "Nyando", will make her own rounds which involve searching for the largest element; Nyando will then deposit this largest \( UNSORTED \) element at position \( n \), pointed to by the other spirit, also known as Aboko. From this point, Aboko will confirm the deposition and shift to the next position for the next but upcoming deposition, which will now be position \( n - 1 \). At this point, Nyando's search space is relatively smaller. She will have to search, in her rounds, from positions 1 until position \( n-2 \) and then she'll deposit the largest element found at the position \( n-1 \) that's pointed to by Aboko. Then Aboko will take another round where he'll point at position \( n-2 \) for deposition and Nyando will search again from positions \( 1 \) to position \( n-3 \). This continues, my Queen, until Aboko reaches position \( 2 \).

As you observed my queen, Aboko's rounds make him to be decreasing the position number. He started from position \( n \), and then went to position \( n-1 \), and then to \( n-2 \) until he stopped at position \( 2 \).

"Why did he stop at position 2?" the Queen asked.

My Queen, as the great Nyando is searching for her elements in the \( UNSORTED \) region, her search space is shrinking, while Aboko's \( SORTED \) region is expanding. Intuitively, as the list is being sorted, more and more unsorted elements are bubbled up to the sorted region. Since the elements are lined up from \( 1...n \), the venerable spirits Aboko and Nyando will grow and shrink their regions until Nyando will have only one element in position \( 1 \) to sort; Aboko will be pointing at the very next position \( 2 \). But one element in its own right is already sorted. However, if the elements at positions \( 1 \) and \( 2 \) are not in order, Nyando can simply exhange them, and the whole list or array or lineup will be completely sorted. Hence, Aboko stops at position \( 2 \) because it leaves only a pair of numbers and they can be easily interchanged if the need arises.

Interestingly, my Queen, the exact nature of the techniques used by Nyando to find the largest in the \( UNSORTED \) region also explains why Aboko will stop at position 2. Nyando, as the gods said, discovered that a natural way to compare a lineup of elements is to use the fact that every element in the lineup, except the first, has a predecessor or someone that comes before it; also, every element, except the last element in the lineup, has a successor or someone after it. Hence, Nyando concluded that she can start from the first element or any given element she's dealing with at a given time, also known as the cursor, and simply compare it with it's successor. If the cursor is bigger than its successor, she'd swap them. Therefore, she'd push the bigger element 1 position towards the \( SORTED \) region. It follows, My Queen, that Nyando's rounds involve comparing successive cursors and advancing them towards the \( SORTED \) region. By some stroke of luck, Nyando's rounds continually advance the biggest element until it is deposited at the position pointed to by Aboko.

My Queen, I've described the operative aspects of this algorithm. With the help of the gods, I managed to write the most essential steps of the process on this stone tablet. Kkaienge presented a dark blue stone tablet to the Queen. There were some lines scribbled on this stone tablet in silvery strokes. It read:

    input: ARRAY, LINEUP, LIST

    for i = n downto 2 do
        for j = 1 to i-1
            if LIST[j] > LIST[j+1]
            swap(LIST[J], LIST[J+1])
        end for
    end for

    output: Sorted LIST

"My goodness!" exclaimed the queen. "Kkaienge," she continued, "what is this and why is it different?"

Oh! My dutiful Queen, Kkaienge replied, the spirits call that pseudocode. It's a collection of the instructions that express the operations that Aboko and Nyando were performing. The line **for i = n downto 2 do** represents the rounds or the job that Aboko, the pointer, was doing. The line **for j = 1 to i-1** represents the rounds that Nyando was doing. The line **if LIST[j] > LIST[j+1]** represents the comparison of neighboring elements that Nyando performed. And the line **swap(LIST[j], LIST[j+1])** expresses the exchange activity that Nyando engages in if the cursor is larger than its successor. That my Queen, is the expression of the Bubble Sort algorithm that the gods blessed us with.

"Thank you, dear Kkaienge. Can you show me how to use this right here and right now?" With pleasure, my Queen, Kkaienge replied.

Suppose, my Queen, that "Efongo" sitting right here plays the role of Aboko. He'd point at the points of deposition and so perform the tasks specified on the line **for i = n downto 2 do**. In fact, Efongo, please come here and I'll instruct you on what to do on our 13 measurements so that we can sort them before our Queen. Efongo came forward. And Nyanga Ni, please come and play the role of Nyando. You would be given the \( UNSORTED \) region to play with and you'd have to transport the largest element to the position Efongo over here is pointing at.

To begin with, here are our 13 elements are:

| ![img]({{site.url}}/images/bsort/list1.png "The original lineup of produce data according to tribe number") |
|:--:|
| *The original lineup of produce data according to tribe number* |

For this problem, my fellow brothers and sisters, we have 13 elements to sort using the Bubble Sort algorithm. Therefore, our \( n \) is 13. Efongo your task now is to point at position 13. You, Efongo, will be in charge of the sorted region. At this point, you only command position \( n \) and no element is sorted so far. As we proceed, marching towards position 2, you will have command over a wider region, while Nyanga Ni will be handing over elements to you and expanding your region; in the same time, she will be shrinking her region of command. Below is a diagram of what Nyanga Ni and Efongo controlled at the start of the process.

|![img]({{site.url}}/images/bsort/list2.png "Nyanfa Ni's and Efongo's regions at start of process")|
|:--:|
| *Nyanfa Ni's and Efongo's regions at start of process* |

Now, Nyanga Ni, your round begins at position \( 1 \) and ends at position \( 12 \). You would start at position \( 1 \). You'd compare the element, 234, with the element at position \( 2 \). In this case, \( 234 \) is bigger than \( 213 \). So we shall exhange them in the lineup. Luckily, the gods provided us with, as shown on the stone tablet, some kind of counter which they called \( j \). This counter should be incremented by \( 1 \) as you take rounds comparing successive pairs of elements. The counter \( j \) is the cursor; it represents the current element you want to compare with its next, right, neighbor. After the exchange, if there is one, you would increase your counter \( j \) by 1. In effect, you would test if \( LIST[j] > LIST[j+1] \); you would then swap if your  pair of elements are out of order. Next, you would increment \( j \) by \( 1 \) and repeat the comparison and or swapping until the value you get by incrementing \( j \) by \( 1 \) becomes equal to the number \( i - 1 \). In the first case, \( i = 13 \). This implies that you would compare consecutive pairs from \( j = 1 \) to \( j = 12 \). You would have to compare the element at position \( 12 \) and the element at position \( 13 \) and effect the swap if they are out of order.

Go on, Nyanga Ni and Efongo. Perform the first step let's all be delighted. Nyanga Ni at once selected the \( 234 \) which is at position \( 1 \). She compared \( 234 \) and \( 213 \). She then swapped them, since the element at position \( 1 \) is bigger. That was her first round. She then incremented \( j \) by \( 1 \). The value of \( j \) became \( 2 \), so Nyanga Ni then compared \( 234 \), which is now at position \( 2 \), with \( 382 \) which is at position \( 3 \). However, \( 382 \) is bigger than \( 234 \), so an  exchange is made. Nyanga Ni then incremented \( j \) by \( 1 \) again and continued her journey. "This is fun", Nyanga Ni exxlaimed. "Wait until we do Heapsort or Merge Sort or any of the more elegant and more performant algorithms the gods revealed to me," Kkaienge replied.

Here is what the Queen saw after the first exhange:

| ![img]({{site.url}}/images/bsort/list3.png "Lineup after Nyanfa Ni swaps elements at positions \( 1 \) and \( 2 \)") |
|:--:|
| *Lineup after Nyanfa Ni swaps elements at positions 1 and  2* |


Now, \( j \) is incremented to position \( 3 \) with an element of \( 382 \). The element, at position \( 4 \), next to \( 382 \), is \( 101 \). Clearly, and swiftly, Nyanga Ni made a swap.


|![img]({{site.url}}/images/bsort/list4.png "Lineup after Nyanfa Ni swaps elements at positions \( 3 \) and \( 4 \)")|
|:--:|
| *Lineup after Nyanfa Ni swaps elements at positions 3 and 4* |



|![img]({{site.url}}/images/bsort/list5.png "Lineup after Nyanfa Ni swaps elements at positions \( 5 \) and \( 6 \)")|
|:--:|
|*Lineup after Nyanfa Ni swaps elements at positions  5 and 6* |



|![img]({{site.url}}/images/bsort/list6.png "Lineup after Nyanfa Ni swaps elements at positions \( 7 \) and \( 8 \)")|
|:--:|
|*Lineup after Nyanfa Ni swaps elements at positions 7 and 8*|



|![img]({{site.url}}/images/bsort/list7.png "Lineup after Nyanfa Ni swaps elements at positions \( 8 \) and \( 9 \)")|
|:--:|
|*Lineup after Nyanfa Ni swaps elements at positions 8 and 9*|



|![img]({{site.url}}/images/bsort/list8.png "Lineup after Nyanfa Ni swaps elements at positions \( 9 \) and \( 10 \)")|
|:--:|
|*Lineup after Nyanfa Ni swaps elements at positions 9 and 10*|



|![img]({{site.url}}/images/bsort/list9.png "Lineup after Nyanfa Ni swaps elements at positions \( 10 \) and \( 11 \)")|
|:--:|
|*Lineup after Nyanfa Ni swaps elements at positions 10 and 11* |



|![img]({{site.url}}/images/bsort/list10.png "Lineup after Nyanfa Ni swaps elements at positions \( 11 \) and \( 12 \)")|
|:--:|
|*Lineup after Nyanfa Ni swaps elements at positions 11 and 12* |

Nyanga Ni is now at position \( 12 \). She can't go any further. She can however perform her last comparison and/or swap.



|![img]({{site.url}}/images/bsort/list11.png "Lineup after Nyanfa Ni swaps elements at positions \( 12 \) and \( 13 \)")|
|:--:|
|*Lineup after Nyanfa Ni swaps elements at positions 12 and 1* |

And by this point, Nyanga Ni has succeeded in depositing the largest element in the correct position, \( 13 \). She will now walk back to begin the second set of rounds, whence she'd find the next largest and deposit this element in the position pointed at by Efongo. Since Nyanga Ni succeeded in effecting a deposition, Efongo shifted the deposit position \( 1 \) less than the former. That is, Efongo decremented the value of \( i \) by \( 1 \).

"Wait a minute, dear Kkainge," the Queen uttered. "Does it mean that the counter \( i \) is reduced downards towards \( 2 \) but at a very slow rate?" Yes my Queen! Efongo decrements the value \( j \) once in a while. Nyanga Ni, on the other hand, quickly walks up from \( 1 \) to \( i-1 \) by incrementing \( j \) by one, but she does so at a higher frequency. Nyanga Ni performs up to \( i-1 \) comparisons before Efongo decrements his counter by 1. That is, Nyanga Ni incremenets \( j \) up to \( i-1 \) times before Efongo makes a single decrement. For Efongo's first round, Nyanga Ni incremented \( j \) 12 times. In the next round, that is when Efongo points to position \( 12 \), Nyanga Ni performed 11 increments of \( j \). A subtle pattern appears; the use of this pattern will become evident later, my dear brethren.

If I may continue, brethen, Nyanga Ni will now go back to position \( 1 \) and she will repeat the whole process again until she deposits the next largest at the position Efongo points to.

Below are the pictures of Nyanga Ni's and Efongo's work. Efongo points at the deposition position with his right hand, and he points at the end of the lineup with his left hand. This marks the boundaries of the \( SORTED \) region.

|![img]({{site.url}}/images/bsort/list12.png "Nyanga Ni commands \( 1..11 \) and Efongo commands \( 12, 13 \)")|
|:--:|
|*Nyanga Ni commands 1..11 and Efongo commands 12, 13*|



|![img]({{site.url}}/images/bsort/list13.png "Lineup after Nyanga Ni swaps elements at positions \( 2 \) and \( 3 \)")|
|:--:|
|*Lineup after Nyanga Ni swaps elements at positions 2 and  3*|



|![img]({{site.url}}/images/bsort/list14.png "Lineup after Nyanga Ni swaps elements at positions \( 5 \) and \( 6 \)")|
|:--:|
|*Lineup after Nyanga Ni swaps elements at positions 5 and 6*|



|![img]({{site.url}}/images/bsort/list15.png "Lineup after Nyanga Ni swaps elements at positions \( 6 \) and \( 7 \)")|
|:--:|
|*Lineup after Nyanga Ni swaps elements at positions 6  and 7*|



|![img]({{site.url}}/images/bsort/list16.png "Lineup after Nyanga Ni swaps elements at positions \( 7 \) and \( 8 \)")|
|:--:|
|*Lineup after Nyanga Ni swaps elements at positions 7 and 8* |



|![img]({{site.url}}/images/bsort/list17.png "Lineup after Nyanga Ni swaps elements at positions \( 8 \) and \( 9 \)")|
|:--:|
|*Lineup after Nyanga Ni swaps elements at positions 8 and 9*|



|![img]({{site.url}}/images/bsort/list19.png "Lineup after Nyanga Ni swaps elements at positions \( 9 \) and \( 10 \)")|
|:--:|
|*Lineup after Nyanga Ni swaps elements at positions 9 and 10*|



|![img]({{site.url}}/images/bsort/list20.png "Lineup after Nyanga Ni swaps elements at positions \( 11 \) and \( 12 \)")|
|:--:|
|*Lineup after Nyanga Ni swaps elements at positions 11 and 12*|


The august Kkaienge continued his commentaries as Nyango Ni and Efongo were busily sorting the tribes data. Kkaienge said it can be evident that this Bubble Sort takes a long time to sort elements. The gods told him it was one of the slowest algorithms, especially if the algorthm has to be used for large lineups. After sometime, Nyanga and Efongo said they were done. Efongo was pointing as position \( 2 \).



|![img]({{site.url}}/images/bsort/list21.png "Lineup after Nyanga Ni and Efongo are done sorting&#x2026;")|
|:--:|
|*Lineup after Nyanga Ni and Efongo are done sorting&#x2026*|

By this point, the Queen expressed her joys with the most brilliant smile. She and her court had succeeded, for the first time in their history, to sort data. It appears tribe number \( 7 \) had the least produce.

Before departing, the Queen asked Kkaienge:

"My dear chief, is it possible to obtain the exact number of comparisons that Nyanga Ni can ever perform in the course of the algorithm for any lineup? Is it also possible to obtain the total number of swaps she performed, too, for any lineup?"

Kkaienge thought for a while and then he responded:

It is very possible, my great Queen. The gods showed me how to count such operations. They called it, *The Analysis of Algorithms* and they reported that the first human to do this a long time ago is called **Don Knuth**. Through analysis of algorithms, the analyst can obtain quantitive information about the cost accrued in the course of running algorithms. Since the Queen was about to depart, Kkaienge promised to demonstrate, in the near future, the art of analyzing algorithms in general, with the assistance and testimony of the analysis of the Bubble Sort algorithm.

The rest of the court were fascinated by the primitive procedure they'd just observed. The Queen obtained the information she requested. Kkaienge thanked the court for their attention and promised to next demonstrate the analysis of the algorithm they just observed.
