# BUSA8090_Assignment1
This is my submissions for BUSA8090 Assignment 1.

My GitHub link: https://github.com/startup-101/BUSA8090_Assignment1

# Question 1
**Written Documentation about Q1**: Reference to Recording 2 of Lecture 2, topic position parameters (slide 14) + Recording 4 of Lecture 2, slide 6.
```
#!/bin/bash
echo "Searching for oldest file"
oldest_file=$(find $HOME -type f -name "*.foo" -o -name "*.goo"  -o -name "*.hoo" -exec grep "$oldest" {} \;)
echo "The oldest file is: $oldest_file"
```

# Question 2
**Written Documentation about Q2**: Reference to Recording 4 of Lecture 2, slides 22-24. 
```
#!/bin/bash
if [ -f ~/funny.sh ];
then
        echo "This is funny";
else
        echo "This is NOT funny";
fi
```

# Question 3
**3a**. <i> Code overview: curl -O filename URL to Wünschiers book <i>

The curl command was used to since it can download files from a remote location, like a webpage!
Additionally, I opted to use -O (vs -o) as it automatically saved case-cp.sh in my current working directory.
```
curl -O case-cp.sh https://link-springer-com.simsrad.net.ocs.mq.edu.au/book/10.1007%2F978-3-642-34749-8
```

**3b**. 
**Written Documentation about Q2**: Reference to Recording 4 of Lecture 2, slides 30-31. Reference to 10.11.2 Time Signal in Computational Biology.
```
#!/bin/bash
time=$(date +%M)
count=0
let count=count+1;

if [[ $minute -gt 0 && $minute -lt 20 ]];
then
        echo "No Chime"
elif [[ $minute -gt 20 && $minute -lt 40 ]];
then
        echo -e "\a"
elif [[ $minute -gt 40 && $minute -lt 60 ]];
then
        echo -e "\a\a"
        sleep 1
fi
```
### -- END OF SUBMISSION --
