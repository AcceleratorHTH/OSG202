# **OSG202 LAB2**
> **Date: 08/06/2022**

**Student:**

- Pham Quoc Trung
- HE171493
- IA1701

**Used Language**
- Bash Script

**Problem Solving**
- Problem:
- Solution:

```console
#!/bin/bash


if [[ $# -eq 1 ]]
then if [[ $1 -le 0 ]]
	then echo "error"
	else
		echo -n "chu vi hv = `expr $1 \* 4`"
	       	echo "; dien tich =  `expr $1 \* $1`"
	fi
elif [[ $# -eq 2 ]]
then if [[ $1 -le 0 || $2 -le 0 ]]
	then echo "error"
	else
		echo -n "chu vi hcn =  `expr $1 \* 2 + $2 \* 2`"
		echo "; dien tich hcn =  `expr $1 \* $2`"
	fi
elif [[ $# -eq 3 ]]
then if	[[ $1 -le 0 || $2 -le 0 || $3 -le 0 ]]
	then echo "error"
	else
		if [[ `expr $1+$2` -gt $3  &&  `expr $2+$3` -gt $1  &&  `expr $1+$3` -gt $2 ]]
		then echo "chu vi tam giac =  `expr $1 + $2 + $3`"
		else 
		echo "error"
		fi
	fi
else 
	echo "error"
fi

```

\
**© 2022,Pham Quoc Trung. All rights reserved.**
