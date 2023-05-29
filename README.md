# Writing_in_a_file
A simple example of how to write in a file 

        text_file = open('inputFile.txt', 'r')
        passed_file = open('passedFile.txt', 'w')
        failed_file = open('failedFile.txt', 'w')
        for line in text_file:
            line_split = line.split()
            if line_split[2] == 'P':
                passed_file.write(line)
            else:
                failed_file.write(line)
        text_file.close()
        passed_file.close()
        failed_file.close()


