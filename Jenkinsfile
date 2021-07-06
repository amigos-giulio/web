@Library('jenkins-shared-library@feature/giulio-testing') _

theMultiPipeline(
    folders: [
        client: [
            _defaults: 'base',
            project: 'web',
            stages: [
                test: [
                    steps: [
                        'docker-compose run web python3 manage.py test'
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
