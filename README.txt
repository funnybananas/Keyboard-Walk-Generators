   
    
Method 2 Usage
--------------

    Commandline Arguments:
    ----------------------
    usage: Combinator.py [-h] [-l [L]] [file_name]

        Combinator: Combine strings into arbitrary length strings

        positional arguments:
          file_name            File with strings of same length

        optional arguments:
          -h, --help           show this help message and exit
          -l [L], -length [L]  Length of final strings
          
    EXAMPLE: To create a dictionary of keyboard walks of length 16 the best results come from combining the seed file into length 8 and then into a 16 length file.

    python Combinator.py 4_Walk_seed.txt -l 8 > 8_Walk.txt
    python Combinator.py 8_Walk.txt -l 16 > 16_Walk.txt

    Executing the above commands should generate a file of around 5GB in size. Then you can input the resulting 16_Walk.txt file and walk.rule file into a password cracker. NOTE: The walk.rule rules were written for oclHashcat, but may work in other crackers such as John. 



