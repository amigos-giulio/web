@Library('jenkins-shared-library@feature/giulio-testing') _

theMultiPipeline(
    folders: [
        client: [
            _defaults: 'base',
            project: 'web',
            stages: [
                build: [
                    steps: [
                        'docker-compose up -d'
                    ]
                ],
                dockerise: [
                    steps: [
                        'echo "No need to dockerise"'
                    ]
                ]
            ]
        ],
        server: [
            _defaults: 'base',
            project: 'web',
            stages: [
                dockerise: [
                    steps: [
                        'echo "No need to dockerise"'
                    ]
                ]
            ]
        ]
    ]
)
