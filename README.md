# Simple_Combo_Counter_Document

```cpp
UComboCounterComponent();

UPROPERTY(EditAnywhere, Category = "SimpleComboCounter")
int ComboCount{};

UPROPERTY(EditAnywhere, Category = "SimpleComboCounter")
int IncrementAmount{};

UPROPERTY(EditAnywhere, Category = "SimpleComboCounter")
int MaxCombo{};

UPROPERTY(EditAnywhere, Category = "SimpleComboCounter")
float ComboTimeout{};


UFUNCTION(BlueprintCallable, Category = "SimpleComboCounter")
void IncrementCombo();

UFUNCTION(BlueprintCallable, Category = "SimpleComboCounter")
int GetCombo();

UFUNCTION(BlueprintCallable, Category = "SimpleComboCounter")
void ResetCombo();

FTimerHandle ComboTimerHandle;

```



## Function: IncrementCombo()
Description: Increases the combo count.
Details:
Resets the combo timer.
Sets a new timer to reset the combo after a specified duration (ComboTimeout).
Increases the combo count as long as it doesn't exceed the maximum combo limit.


## Function: GetCombo() -> int
Description: Returns the current combo count.
Return Value: Current combo count as an int.


## Function: ResetCombo()
Description: Resets the combo count.
