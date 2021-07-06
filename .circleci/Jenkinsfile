@Library('jenkins-shared-library@feature/giulio-testing') _

theMultiPipeline(
    folders: [
        client: [
            _defaults: 'base',
            project: 'simple-project-multi-client'
            dockerise: [
                steps: [
                    'echo "No need to dockerise"'
                ]
            ]
        ],
        server: [
            _defaults: 'base',
            project: 'simple-project-multi-server'
            dockerise: [
                steps: [
                    'echo "No need to dockerise"'
                ]
            ]
        ]
    ]
)