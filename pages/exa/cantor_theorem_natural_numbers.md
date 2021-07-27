Alice and Bob are discussing how big is the set $\mathcal{P}(\N)$, that is, the collection of all subsets of the natural numbers. The more they think about it, the more they realise this collection is really huge! Examples and examples of subsets of $\N$ come to their minds:

<ul>
  <li>The even numbers: $2 \N=\{0,2,4,6,8,10,12,14,...\}$</li>
  <li>The numbers between 50 and 83: $[50,83]=\{50, 51, 52,...,81, 82,83\}$</li>
  <li>The empty subset: $\varnothing=\{\}$</li>
  <li>The prime numbers: $Prime=\{2,3,5,7,11,13,17,19,23,29,31,...\}$</li>
  <li>Bob's age (just one element!): $BobAge=\{14\}$</li>
  <li>The nonprime numbers: $NonPrime=\{0,1,4,6,8,9,10,12,14,15,16,18,20,21,22,24,25,26,27,28,30,32,...\}$</li>
  <li>The set of lucky numbers among Alice and Bob's friends: $LuckyNumbers=\{3,4,5,6,7,12,13,16,99,777,12345\}$</li>
  <li>All the numbers! $\N=\{0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,...\}$</li>
  <li>The powers of $2$: $PowersTwo=\{1,2,4,8,16,32,64,128,256,512,1024,...\}$</li>
  <li> ... and so on ...</li>
</ul>

Alice and Bob wonder whether this collection is _countable_, that is, whether one may hypothetically write down all the subsets of $\N$ in a list without leaving any unnoticed. Alice is somewhat prone to believe that this is not possible; Bob, on the other hand, is sure about this collection being countable and also says he conceives a strategy to achieve this ordering

"Show me then!" - says Alice 

And Bob takes a piece of paper and starts to write down

$$2 \N=\{0,2,4,6,8,10,12,14,...\}$$
$$[50,83]=\{50, 51, 52,...,81, 82,83\}$$
$$\varnothing=\{\}$$
$$Prime=\{2,3,5,7,11,13,17,19,23,29,31,...\}$$
$$BobAge=\{14\}$$
$$NonPrime=\{0,1,4,6,8,9,10,12,14,15,16,18,20,21,22,24,25,26,27,28,30,32,...\}$$
$$LuckyNumbers=\{3,4,5,6,7,12,13,16,99,777,12345\}$$
$$\N=\{0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,...\}$$
$$PowersTwo=\{1,2,4,8,16,32,64,128,256,512,1024,...\}$$
$$...$$
$$...$$
$$...$$

"Oh, this gonna be dull" - thinks Alice. She's not very confident about Bob being able to write down infinitely many items in a piece of paper... but even if he is able, she won't check the infinite list to ensure no subset of $\N$ is left. "There must be a smarter way"

And she remembers - [Cantor's Theorem]( thm | cantor_theorem ). How could she have overlooked it?

Yes, when trying to count the subsets of $\N$, Bob is building a map $g:\N\longrightarrow\mathcal{P}(\N)$. He hasn't ended yet, but says that has a rule to write down everything

<table>
  <thead>
    <tr>
      <td>$a$</td>
      <td>$g(a)$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>$0$</td>
      <td>$2 \N=\{0,2,4,6,8,10,12,14,...\}$</td>
    </tr>
    <tr>
      <td>$1$</td>
      <td>$[50,83]=\{50, 51, 52,...,81, 82,83\}$</td>
    </tr>
    <tr>
      <td>$2$</td>
      <td>$\varnothing=\{\}$</td>
    </tr>
    <tr>
      <td>$3$</td>
      <td>$Prime=\{2,3,5,7,11,13,17,19,23,29,31,...\}$</td>
    </tr>
    <tr>
      <td>$4$</td>
      <td>$BobAge=\{14\}$</td>
    </tr>
    <tr>
      <td>$5$</td>
      <td>$NonPrime=\{0,1,4,6,8,9,10,12,14,15,16,18,20,21,22,24,25,26,27,28,30,32,...\}$</td>
    </tr>
    <tr>
      <td>$6$</td>
      <td>$LuckyNumbers=\{3,4,5,6,7,12,13,16,99,777,12345\}$</td>
    </tr>
    <tr>
      <td>$7$</td>
      <td>$\N=\{0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,...\}$</td>
    </tr>
    <tr>
      <td>$8$</td>
      <td>$PowersTwo=\{1,2,4,8,16,32,64,128,256,512,1024,...\}$</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
    </tr>
  </tbody>
</table>

and according to Cantor's Theorem, $g$ will never be surjective, that is, Bob won't be able to write down _all_ subsets of $\N$! She's right! Come on, let's follow the argument of Cantor's proof.

Among the natural numbers, the are some that belong to its associated subset, but others not

<table>
  <thead>
    <tr>
      <td>$a$</td>
      <td>$g(a)$</td>
      <td c>$a\in g(a)$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>$0$</td>
      <td>$2 \mathbb{N}=\{\hl{0},2,4,6,8,10,12,14,...\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$1$</td>
      <td>$[50,83]=\{50, 51, 52,...,81, 82,83\}$</td>
      <td c>::cross::</td>
    </tr>
    <tr>
      <td>$2$</td>
      <td>$\varnothing=\{\}$</td>
      <td c>::cross::</td>
    </tr>
    <tr>
      <td>$3$</td>
      <td>$Prime=\{2,\hl{3},5,7,11,13,17,19,23,29,31,...\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$4$</td>
      <td>$BobAge=\{14\}$</td>
      <td c>::cross::</td>
    </tr>
    <tr>
      <td>$5$</td>
      <td>$NonPrime=\{0,1,4,6,8,9,10,12,14,15,16,18,20,21,22,24,25,26,27,28,30,32,...\}$</td>
      <td c>::cross::</td>
    </tr>
    <tr>
      <td>$6$</td>
      <td>$LuckyNumbers=\{3,4,5,\hl{6},7,12,13,16,99,777,12345\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$7$</td>
      <td>$\mathbb{N}=\{0,1,2,3,4,5,6,\hl{7},8,9,10,11,12,13,14,15,...\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$8$</td>
      <td>$PowersTwo=\{1,2,4,\hl{8},16,32,64,128,256,512,1024,...\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
      <td c>::question_mark::</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
      <td c>::question_mark::</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
      <td c>::question_mark::</td>
    </tr>
  </tbody>
</table>

So we have to focus on the set of "red numbers"

$$\color{#DD2C00}{B=\{1,2,4,5,...\}}$$

"Bob! I know this subset is not contained in your list!"

Bob rolled his eyes - "How do you know, if I haven't even finished writing down?"

But Alice explains her argument. "Imagine $B$ is in the list, as the image of some number $b$. Now, is $b$ a _green number_ or a _red number_?"

<table>
  <tr>
    <td>$b$</td>
    <td>$B=\{1,2,4,5,...,\mathbf{\color{#00C853}{b}},...\}$</td>
    <td>::check::</td>
  </tr>
  <tr>
    <td>$b$</td>
    <td>$B=\{1,2,4,5,...\}$</td>
    <td>::cross::</td>
  </tr>
</table>

"Neither makes sense, because $B$ is exactly the set of red numbers!" said Alice. "Isn't this clever?"

"Yikes, you're right!", said Bob finally...