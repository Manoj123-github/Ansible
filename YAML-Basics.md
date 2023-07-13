# YAML Basics for Ansible
Ansible uses YAML syntax for expressing Ansible playbooks. Ansible uses YAML because it is very easy for humans to understand, read and write when compared to other data formats like XML and JSON.

# key-value pair
YAML uses simple key-value pair to represent the data. The dictionary is represented in key: value pair.

**Note − There should be space between : and value.**

# Example: A student record
<pre>
  --- #Optional YAML start syntax 
Manoj: 
   name: Manoj Yadav 
   rollNo: 34 
   div: A
   sex: male 
… #Optional YAML end syntax 
</pre>


# You can also use abbreviation to represent dictionaries.

# Example
<pre>
Manoj: {name: Manoj Yadav, rollNo: 34, div: A, sex: male}
</pre>


# Representing List
We can also represent List in YAML. Every element(member) of list should be written in a new line with same indentation starting with “- “ (- and space).

**Example**
<pre>
---
countries:  
   - America 
   - China 
   - Canada 
   - Iceland 
…
</pre>



You can also use abbreviation to represent lists.

Example
<pre>
Countries: [‘America’, ‘China’, ‘Canada’, ‘Iceland’] 
</pre>



# List of Dictionaries

Example

<pre>
---  
- james: 
   name: james john 
   rollNo: 34 
      div: B 
   sex: male 
   likes: 
      - maths 
      - physics 
      - english 

- robert: 
      name: robert richardson 
      rollNo: 53 
      div: B 
      sex: male 
   likes: 
      - biology 
      - chemistry 
…  
</pre>



