# Malware Memory Analysis

Obfuscated malware is malware that hides to avoid detection and extermination. This repo aims to find a way to detect malware through memory analysis.

## Datasets

The obfuscated malware dataset, [CIC-MalMem-2022](https://www.unb.ca/cic/datasets/malmem-2022.html), is designed to test obfuscated malware detection methods through memory. The dataset was created to represent as close to a real-world situation as possible using malware that is prevalent in the real world. Made up of Spyware, Ransomware and Trojan Horse malware, it provides a balanced dataset that can be used to test obfuscated malware detection systems.

This dataset uses debug mode for the memory dump process to avoid the dumping process to show up in the memory dumps. This works to represent a more accurate example of what an average user would have running at the time of a malware attack.

## Additional Features

The following additional features are designed for obfuscated malware detection.
- Malfind - commitCharge - Total number of Commit Charges
- Malfind - protection - Total number of protection
- Malfind - uniqueInjections - Total number of unique injections
- Ldrmodule - avgMissingFromLoad - The average amount of modules missing from the load list
- Ldrmodule - avgMissingFromInit - The average amount of modules missing from the initilization list
- Ldrmodule - avgMissingFromMem - The average amount of modules missing from memory
- Handles - port - Total number of port handles
- Handles - file - Total number of file handles
- Handles - event - Total number of event handles
- Handles - desktop - Total number of desktop handles
- Handles - key - Total number of key handles
- Handles - thread - Total number of thread handles
- Handles - directory - Total number of directory handles
- Handles - semaphore - Total number of semaphore handles
- Handles - timer - Total number of timer handles
- Handles - section - Total number of section handles
- Handles - mutant - Total number of mutant handles
- Process View - pslist - Average false ratio of the process list
- Process View - psscan - Average false ratio of the process scan
- Process View - thrdproc - Average false ratio of the third process
- Process View - pspcid - Average false ratio of the process id
- Process View - session - Average false ratio of the session
- Process View - deskthrd - Average false ratio of the deskthrd
- Apihooks - nhooks - Total number of apihooks
- Apihooks - nhookInLine - Total number of in line apihooks
- Apihooks - nhooksInUsermode - Total number of apihooks in user mode

## Stacked Framework

### Layer 1
* Random Forest
* SVM
* Decision Tree
* Naive Bayes

### Layer 2
* LogisticRegression
