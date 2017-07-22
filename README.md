# Simulating an AI

## Memory
- Person
- Place
- Thing
- Activity
- Place
- Mood

## Next steps
- select personalities
  - Harry Potter
  - Calvin and Hobbes
  - Seinfeld

- find data sources
  - for memories
  - for voice
  - for images

## Identify Tools to parse memories


## Memory

Dates are all in ISO 8601 Format  
https://en.wikipedia.org/wiki/ISO_8601#UTC  
(http://xkcd.com/1179/)

```
{
    memory: '', 
    node:   
        {
            name: '', 
            label: '',
            imageURL: '', 
            iconURL: '',
	          created: '2016-04-14T17:02:34.000Z',
            updated: '2016-04-14T17:02:34.000Z'
        }, 
    relation: 
        {
            name: '',
            weight: 0.5,
            joy: 0.2,
            fear: 0.1, 
            surprise: 0.0, 
            sadness: 0.0, 
            disgust: 0.0, 
            anger: 0.3
        }
    concepts: [
        {
            node:
                {
                    concept: Person,
                    name: 'mom', 
                    label: 'mom', 
                    iconURL: '', 
                    imageURL: ''
                },
            relation:
                {
                    relation: 'Has_Person',
                    name: '', 
                    weight, 0.4, 
                    originType: 'OriginUserDefined', 
                    iconURL: '',
                    imageURL: '',
                    joy: 0.0,
                    fear: 0.0, 
                    surprise: 0.0, 
                    sadness: 0.0, 
                    disgust: 0.0, 
                    anger: 0.0
                }
        }
    ], 
    narrative: {
        node: {
            name: '',
            label: 'Lunch with Mom',
            text: 'Went to have lunch with my mom',
            created: '2016-04-14T17:02:34.000Z',
            updated: '2016-04-14T17:02:34.000Z'
        }, 
        relation: {
            weight: 0.5
        }
    }
}
```

