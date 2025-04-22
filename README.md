Install Steam on runner
=======================

```yaml
      - uses: gbraad-actions/install-steam-action@main
      - name: Login to Steam
        run: |
          steam -login ${{ secrets.STEAM_USERNAME }} ${{ secrets.STEAM_PASSWORD }}

      - name: Hang around
        run: |
          Start-Sleep -Seconds 21600
```
