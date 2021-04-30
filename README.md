#
            - exec:
                arguments:
                - clone
                - git@gitlab.z5x.tech:z5x-tech/zeezest/zeezest-web.git
                command: git
                run_if: passed
            - exec:
                arguments:
                - sts
                - get-caller-identity
                command: aws
                run_if: passed
