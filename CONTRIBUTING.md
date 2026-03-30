# Contributing to Universal Calculator Hub

Thanks for your interest in contributing! 🎉

## How to Contribute

### Adding a New Calculator

1. Fork the repo
2. Add your calculator definition to `app.js` in the `CATS` object
3. Add the calculator logic to the `FN` object
4. Test locally with `npm start`
5. Submit a PR with a clear description

### Calculator Structure

```javascript
// In CATS object
{id:'my_calc',icon:'🔢',name:'My Calculator',desc:'Short description'}

// In FN object
my_calc(){
  const val = +g('c0'); // Get input value
  if(!val) return;
  r([{l:'Result',v:val*2,big:1}]); // Display result
}

// In buildUI function (M object)
my_calc:`<div class="f"><label>Input</label><input id="c0" type="number"/></div>${B}<div id="R"></div>`
```

### Code Style

- Use concise variable names for minification
- Keep functions small and focused
- Test edge cases (0, negative, empty input)
- Use existing patterns from other calculators

### Testing

```bash
npm start
# Open http://localhost:3000
# Test your calculator thoroughly
```

### Pull Request Guidelines

- One calculator per PR
- Clear commit messages
- Update CHANGELOG.md
- Test on mobile and desktop
- Ensure offline functionality works

## Bug Reports

Open an issue with:
- Calculator name
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

## Questions?

Open a discussion or issue — we're happy to help!
