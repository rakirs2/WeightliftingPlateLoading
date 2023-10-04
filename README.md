# Olympic Lifting Weight Loader
Create's a program that generates a visual for the plates needed to load a given bar.

## Considerations
- [ ] Must have a toggle for mens bar and women's bar
- [ ] Clips vs competition clips
- [ ] Plates must be loaded properly
- [ ] Program must work with all numbers from empty bar to current world record clean and jerk + 5 kg for men and women
- [ ] Must follow competition loading [rules](https://iwf.sport/wp-content/uploads/downloads/2020/01/IWF_TCRR_2020.pdf) for both competition and training
- [ ] If a weight is above the men's and women's heavy weight world records, print "Are you sure you're not using pounds?"

The fundamental method must be:
```C#
string CalculateBarWeights(bool isWomensBar, bool isCompetition){
}
```

## Representation
| Item        | Weight  Kg   | Representation |
|--------------|-----------|------------|
| Women's Bar | 15     | -----       |
| Men's Bar      | 20  | =====       |
| Competition Clips     | 2.5 |C      |
| Training Clips      | 0 | c      |
| White changeplate   | 0.5  | w      |
| Green changeplate    | 1  | g       |
| Yellow change plate  | 1.5  | y       |
| Blue change plate  | 2  | b       |
| Red Change plate  | 2.5  | r       |
| White     | 5  | W       |
| Green    | 10  | G       |
| Yellow   | 15  | Y       |
| Blue   | 20  | B       |
| Red   | 25  | R       |

## Solution tips and tricks
This solution comes with a basic test suite that checks a few weights. It is not complete. Feel free to add as many tests as you see fit.

## Examples
### 100 mens, competition clips

CrGR=====RGrC

### 100 mens, training clips

cYR=====RYc

### 100 women's, competitionClips

CYR-----RYC



## Program examples

```
Is this a mens bar?
y
Is this a competition?
y
What is the weight?
100

Your bar is:
CrGR=====RGrC
```

```
Is this a mens bar?
n
Is this a competition?
y
What is the weight?
100

Your bar is:
CYR-----RYC
```

```
Is this a mens bar?
n
Is this a competition?
y
What is the weight?
1000

"Are you sure you're not using pounds?"
```


