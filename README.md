public:
    int binary_to_decimal(const string& binary_str) {
        // Code here.
        int decimal = 0;
        int n = binary_str.size();
        for(int i = n-1; i>=0; i--){
            if(binary_str[i] == '1'){
                decimal += (1 << (n - 1 - i));
            }
        }
        return decimal;
    }
};
