# todo-java-infra

## Prerequisites

1.  Create namespace

    ```
    oc new-project <namespace>
    ```

    Example:

    ```
    oc new-project todo-dev
    ```

2.  Create a Image Pull Secret for Quay.io
    ```
    oc create secret docker-registry \
        --docker-server=quay.io \
        --docker-username=<your-username> \
        --docker-password=<your-token> \
        --docker-email=<your-email> \
        quay
    ```

    Example:
    
    ```
    oc create secret docker-registry \
        --docker-server=quay.io \
        --docker-username=rh_rh+robot \
        --docker-password=KASAF239821392HAGSJAGSJOIQWQ2763782632ASUYT \
        --docker-email=secangkirkopipanas@gmail.com \
        quay
    ```
