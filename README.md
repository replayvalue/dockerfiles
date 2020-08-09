## Dockerfiles

This is a collection of Dockerfiles that build the containers needed by Replay Value's various CI/CD processes.

### firebase-emulator

This is an extension of the nodejs container, with the firebase emulators preinstalled. This is useful for running integration tests that require the use of the emulator.

To build this image, run:

    docker build ./firebase-emulator/ -t replayvalue/firebase-emulator:<version-tag>
    docker push replayvalue/firebase-emulator
