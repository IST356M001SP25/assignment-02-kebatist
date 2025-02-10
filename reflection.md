# Reflection

Student Name:  name
Sudent Email:  email

## Instructions

Reflection is a key activity of learning. It helps you build a strong metacognition, or "understanding of your own learning." A good learner not only "knows what they know", but they "know what they don't know", too. Learning to reflect takes practice, but if your goal is to become a self-directed learner where you can teach yourself things, reflection is imperative.

- Now that you've completed the assignment, share your throughts. What did you learn? What confuses you? Where did you struggle? Where might you need more practice?
- A good reflection is: **specific as possible**,  **uses the terminology of the problem domain** (what was learned in class / through readings), and **is actionable** (you can pursue next steps, or be aided in the pursuit). That last part is what will make you a self-directed learner.
- Flex your recall muscles. You might have to review class notes / assigned readings to write your reflection and get the terminology correct.
- Your reflection is for **you**. Yes I make you write them and I read them, but you are merely practicing to become a better self-directed learner. If you read your reflection 1 week later, does what you wrote advance your learning?

Examples:

- **Poor Reflection:**  "I don't understand loops."   
**Better Reflection:** "I don't undersand how the while loop exits."   
**Best Reflection:** "I struggle writing the proper exit conditions on a while loop." It's actionable: You can practice this, google it, ask Chat GPT to explain it, etc. 
-  **Poor Reflection** "I learned loops."   
**Better Reflection** "I learned how to write while loops and their difference from for loops."   
**Best Reflection** "I learned when to use while vs for loops. While loops are for sentiel-controlled values (waiting for a condition to occur), vs for loops are for iterating over collections of fixed values."

`--- Reflection Below This Line ---`
Hello all, 
I wanted to address one particular issue I had with this program that stumped me a lot. The error read 

        for text, expected in tests:
            print(f"Testing: {text}")
            print(f"EXPECTED: {expected}")
            actual = parse_packaging(text)
            print(f"ACTUAL  : {actual}")
>           assert actual == expected
E           AssertionError: assert [{'eggs': 1}, {'carton': 1}] == [{'eggs': 12}, {'carton': 1}]
E             
E             At index 0 diff: {'eggs': 1} != {'eggs': 12}
E             Use -v to get more diff

This error was particularly confusing becuase despite tlaking it out and using copilot I was unable to understand the error within my method and string logically. The perimeters were incorrect but my code seemed very logical to me. With the help of Copilot (all honesty) I was able to understand that the issue was me using strip in place of spilt. 

My code snippet:
    quantity = int(item.split()[0])
        item = item.split()[1].strip()

The behavior of my code was compleety different. Strip removes the whitespac froma  string but it cannot spilt the string into parts. This is somethign that I want to understand better as a result of this assignment. Previously, I thought I was more familiar with Strip and Spilt in the context of an assignment. I foten find myself struggling to implement my coding skills and understanding in these assignments. While Copilot is very helpful and I enjoy it-- I think extra help alongside Professor would help me. 

For each data package we spilt up everything and then sort it based on the first character and the value. By extracting the quantity and item, it takes the first part, an idex. This actions ensure that an item will contain the quantity of the item and its name. You spilt the item again and again and remove any excess whiitespaces. It took a long time to understand why I needed to spilt this multiple times and then eventually I was able to implement the append feature to bring it to the dictionary. I used Copilot to explain that it converts a hierarchy into a structured dictionary.  
The three other tests were not bad at all and if anything they made more logical sense to me. Logic is very big part of my learning methods and how I build code projects. I was able to pass three of the tests which threw my off. Because the others things were quite easy and simple to understand so I passed those tests easily. 

Onto Part 2, 
I did not understand the directions at first, but that was becuase I was in the wrong file. But once I found it, I inputed json files and and then from the packages I inserted everythign that I just coded in the packaging.py. My code reads every single line and then strips it down and inputs the amount of packages to make the total units. My program retrieves the number of units. 
 
 with open('data/packaging.json', 'w') as f:
            json.dump(packages, f, indent=4)

This final pieces of code inputs everything into the JSON file in the data folder. The term 'as f' is a fall back if the program is unable to reach the JSON file it will store it as the variable f. Packages are the list of parsed packages that were organized in the first portion of this project. The JSOn files makes my code easily accesible to be read and processed by other programs to exchange that "parsed package". 

I really enjoyed this project overall becuase it was challenging by using strip, spilt, and the JSON dumping files. I would like to have Professor Angela explain this to me a bit more though. 

