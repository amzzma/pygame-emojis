# pygame-emojis

A simple Python module to display emojis in your Pygame projects.

Installation

To install the pygame-emojis module, follow these steps:

  Download the pygame_emojis.py file from the GitHub repository.
  Place the file in your project directory.

## Usage

To use the emojis in your game, you need to import the pygame_emojis module and use the provided functions to load and render emojis.

```py
import pygame
import pygame_emojis

# Initialize Pygame and create a window
pygame.init()
screen = pygame.display.set_mode((640, 480))

# Load and render emojis
emojis = pygame_emojis.emojis(screen)
emojis.render_text_and_emojis("Hello /e😀/e /e👍/e", (255, 255, 255), (0, 0), 60)

# Update the display
pygame.display.flip()

# Main loop
running = True
while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

# Quit Pygam
pygame.quit()
```

## Displaying Emojis

To display an emoji, you need to enclose it with /e and add a space between each /e sequence. For example:

```
"Hello /e😀/e /e👍/e"
```

This will display the text "Hello" followed by the grinning face emoji and the thumbs up emoji.
