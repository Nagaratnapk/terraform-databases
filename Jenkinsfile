@Library('robot-shared-library@main') _

env.REPONAME="terraform-databases"

terraform()




// pipeline {
//     agent any    
//     parameters {
//          choice(name: 'ENV', choices: ['dev', 'prod'], description: 'Chose Environment') 
//          choice(name: 'ACTION', choices: ['apply', 'destroy'], description: 'Chose Action')
//     }
//     stages {
//         stage('Terraform Init') {
//             steps {
//                 sh "terrafile -f env-${ENV}/Terrafile"  
//                 sh "terraform init -backend-config=env-${ENV}/${ENV}-backend.tfvars"
                    
//             }
//         }

//         stage('Terraform Plan') {
//             steps {
//                 sh "terraform plan -var-file=env-${ENV}/${ENV}.tfvars"
                    
//             }
//         }

//         stage('Terraform Apply') {
//             steps {
//                 sh "terraform ${ACTION} -var-file=env-${ENV}/${ENV}.tfvars -auto-approve"
                    
//             }
//         }
//     }
// }