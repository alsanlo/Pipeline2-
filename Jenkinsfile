pipeline
{
        agent any
        stages
        {
                stage('Primer paso')
                {
                        steps
                        {
                                echo "Primer paso"
                        }
                }
                stage('Pasos Paralelos')
                {
                        parallel
                        {
                                stage('Segundo primer paso')
                                {
                                        steps
                                        {
                                                echo "paso 2.1"
                                        }
                                }
                                stage('Segundo segun paso')
                                {
                                        steps
                                        {
                                                echo "paso 2.2"
                                        }
                                } 
                        }
                }
                stage('Segundo primer paso')
                {
                        steps
                        {
                                echo "Paso 3"
                        }
                } 
        }
}
