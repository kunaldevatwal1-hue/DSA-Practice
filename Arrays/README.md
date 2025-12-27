
// Problem: Reverse an array
// Link: https://leetcode.com/problems/reverse-array/
// Approach:
// 1. Use two pointers (start & end)
// 2. Swap elements
// 3. Move pointers inward
//
// Time Complexity: O(n)
// Space Complexity: O(1)

#include <bits/stdc++.h>
using namespace std;

int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int n = 5;

    int l = 0, r = n - 1;
    while (l < r) {
        swap(arr[l], arr[r]);
        l++;
        r--;
    }

    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";
    }
}
