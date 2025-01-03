# Videos Inspector

![imagem](https://github.com/user-attachments/assets/b136ad6b-fb7a-4731-bde7-9925e2d8e712)


## For what is it about to
This project has a specific goal which is to inspect Youtube videos aimed to obtain information about thier transcription.
It is simple, checks if the video has transcription, which languages and whether it is autogenerated.

## How does it work
The project receives an excel file and retrives another one, so it is impotant to certify that the Youtube videos links are under the **teaser do youtube** column, such as:

 another column      | teaser do youtube |
---------------------|-------------------|
 value 1             | link 1            |
 value 2             | link 2            |
 value 4             | link 3            |

And than starts inspecting each video.

## How to run
There are two ways, using the UI resource, or using by command line.

### UI way
Since it is a Flask app you can clone and run as you expect for a Flask project. Otherwise, with docker compose installed you can just run at the root of the project: 

```
make up
```

### Command line way

With python installed start a venv

```
python -m venv venv
```
Activate it according to your OS, as you can see [here](https://python.land/virtual-environments/virtualenv).

Now just install the requirements:
```
pip install -r requirements.txt
```

And at the root the project save your excel and run the command providing the file name with no extension (.xlsx):
```
python3 executor.py {file_name}
```

### Et Voilà!
