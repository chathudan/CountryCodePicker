# CountryCodePicker

CountryCodePicker will help users to 

1. Search and select Country 
2. Get selected counry's country name,code,currency and dial code (Sri Lanka,LK,LKR,+94)

<img src="https://github.com/chathudan/CountryCodePicker/raw/master/screens/AndroidCountryCodePicker.png" width="200">
<img src="https://github.com/chathudan/CountryCodePicker/raw/master/screens/AndroidCountryDialCodePicker.png" width="200">
<img src="https://github.com/chathudan/CountryCodePicker/raw/master/screens/AndroidCountryDialCodePickerDialog.png" width="200">



## Usage

#####CountryCodePicker on own layout 



```javascript
FragmentManager manager = getSupportFragmentManager();
FragmentTransaction transaction = manager.beginTransaction();

CountryPicker picker = new CountryPicker();

transaction.replace(R.id.home, picker);
transaction.commit();
```


#####CountryCodePicker as Android Dialog 



```javascript 
 CountryPicker picker = CountryPicker.newInstance("SelectCountry");
 picker.show(getSupportFragmentManager(), "COUNTRY_CODE_PICKER");
```


#####CountryPickerListener to get selected country's details



```javascript 
picker.setListener(new CountryPickerListener() {
    @Override
    public void onSelectCountry(String name, String code, String dialCode) {
    }
});
```

