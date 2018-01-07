# Meltdown and Spectre : CPU vulnerabilities — Explained and Exploited

## Systems Affected :

CPU hardware implementations

## Description :
Meltdown and Spectre are the names of two serious security flaws that have been found within computer processors. They could allow hackers to steal sensitive data without users knowing, one of them affecting chips made as far back as 1995.

## What are Meltdown and Spectre ?

Meltdown is a security flaw that could allow hackers to bypass the hardware barrier between applications run by users and the computer’s core memory, which is normally highly protected.
Spectre is slightly different. It potentially allows hackers to trick otherwise error-free applications into giving up secret information.
- Meltdown Attack paper : https://meltdownattack.com/meltdown.pdf
- Spectre Attack paper : https://spectreattack.com/spectre.pdf

## Exploitation : [for test purposes only]

This test is conducted on a machine with the following CPU architecture :

![alt text](https://github.com/jarmouz/spectre_meltdown/blob/master/ls_cpu.png)

## Spectre CVE-2017–5753 and CVE-2017–5715 :

PoC from Spectre Attacks: Exploiting Speculative Execution (https://spectreattack.com/spectre.pdf) :

- Download Spectre code from github
- Compile the C program with : gcc spectre.c

![alt text](https://github.com/jarmouz/spectre_meltdown/blob/master/gcc_spectre.png)

- Execute a.out with : ./a.out

![alt text](https://github.com/jarmouz/spectre_meltdown/blob/master/spectre_exec.png)


## Meltdown CVE 2017–5754 :

- Download the Exploit from github : https://github.com/paboldin/meltdown-exploit
git clone https://github.com/paboldin/meltdown-exploit.git

- Compile the exploit with make command

- Execute run.sh :

![alt text](https://github.com/jarmouz/spectre_meltdown/blob/master/meltdown_exploit.png)

## References :

- CVE-2017–5753, CVE-2017–5715, and CVE-2017–5754 (Meltdown and Spectre) Windows antivirus patch compatibility : https://docs.google.com/spreadsheets/d/184wcDt9I9TUNFFbsAVLpzAtckQxYiuirADzf3cL42FQ/htmlview?usp=sharing&sle=true
- https://www.theguardian.com/technology/2018/jan/04/meltdown-spectre-computer-processor-intel-security-flaws-explainer
- https://meltdownattack.com/
- https://github.com/hannob/meltdownspectre-patches


