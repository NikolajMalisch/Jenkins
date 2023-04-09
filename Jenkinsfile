pipeline {

    agent any  // Run the pipeline on any available agent

    stages {

        stage('Folder with txt file') {  // Define a stage to create a folder and a text file inside it

            steps {

                sh '''
                file="folder1"
                if [ -d "$file" ] ; then  // Check if the folder already exists
                rm -d -r "$file"         // If it does, remove it
                fi
                ls                        // List the contents of the current directory
                mkdir folder1             // Create a new folder called "folder1"
                ls                        // List the contents of the current directory again
                cd folder1                // Change into the "folder1" directory
                touch text.txt            // Create a new empty file called "text.txt"
                ls                        // List the contents of the "folder1" directory
                '''

            }

        }

    }

}
