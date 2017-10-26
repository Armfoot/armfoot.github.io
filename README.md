## Arm + foot

### Question of ~~the day~~ a lifetime

- Why do I need an entire body?

### Daily routine

    fetch('plans.txt')
    .then(response => response.text())
    .then(plans => {
      for(let action of plans.split('\n')){
        if(let direction = action.isMovement()) {
          Armfoot.jump(direction);
        } else {
          switch(action.interaction) {
            case 'wave':
            case 'type':
            case 'play the piano':
              Armfoot.wiggleFingers();
              break;
            case 'workout':
            case 'fetch':
            case 'massage':
              Armfoot.grabAndRelease();
              break;
            case 'hide':
              Armfoot.digHoleAndPlaceHandInside();
              break;
            default:
              Armfoot.grabFootAndRoll();
          }
        }
      }
    });
    
Version 1.0 (fork needed)
